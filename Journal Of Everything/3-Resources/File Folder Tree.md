#git #bash
Output the file-folder structure to a text file for analysis and documentation.

To create a file-folder tree text file on windows git-bash, download [git tree.exe](https://superuser.com/questions/531592/how-to-add-the-tree-command-to-git-bash-in-windows)
## Basic 
```tree > directory_structure.txt```

```tree -a > directory_structure.txt       # Include hidden files```

```tree -d > directory_structure.txt       # Show only directories```

```tree --charset=ASCII > directory_structure.txt # Use ASCII characters (more compatible)```

```tree -L 2 > directory_structure.txt     # Limit depth to 2 levels```

```tree -aC > directory_structure.txt # Show all files with colorization indicators```

If you want to exclude certain patterns (like git files):
```tree -I "node_modules|.git" > directory_structure.txt```

For a more detailed output including file sizes and permissions:
```tree -a --du -h > directory_structure.txt```
