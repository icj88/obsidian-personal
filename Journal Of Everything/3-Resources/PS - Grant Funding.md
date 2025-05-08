
Fund 100 == "General Fund"
Fund 300, 330 == "Federal Fund"


To determine if an employee has grant funding use the following resources:

1. Menu > UVM Reports > Commitment Accounting > Labor Distribution
2. Only critical field is the Fiscal year or date range option
3. Run report, particularly the 'detailed' UVKR091 report

The following R functions handle this dataset:

```R
strip_extraneous_chars <- function(df) {
  for (col in names(df)) {
    if (is_character(df[[col]])) {
      df[[col]] <- str_remove_all(df[[col]], "=\"")
      df[[col]] <- str_remove_all(df[[col]], "\"")
    }
  }
  
  return(df)
}
```

```R
process_pr_data <- function(df) {
  # filter to the earlier paydate in the dataset for each person
  df_su <- df_su %>%
    group_by(Emplid) %>%
    filter(`Check Date` == min(`Check Date`)) %>%
    ungroup()

  df_su <- mutate(df_su,
                  is_grant = substr(`PC BU`, 1, 1) == "G",
                  is_grant = if_else(is.na(is_grant), FALSE, is_grant)) %>%
    filter(`Earnings Descr` %in% c("Regular Pay", "Contract Regular Earnings"),
           Earnings > 50 | Earnings < -50)

  return(df_su)
}
```

