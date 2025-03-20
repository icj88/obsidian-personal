Remove Blanks on 'From Job Title'
Remove 'To Annual Rate' == 0 records

## Identify Promotions
Join FSCM dept rollup from *UV_TREENODE_VW*  see *UV_ICJ_FSCM_LOOKUP* query

Promotion defined as 
	FSCM Unit To == FSCM Unit From 
	'To Annual Rate' - 'From Annual Rate' > 0

Review very small nominal and/or percentage increases.           