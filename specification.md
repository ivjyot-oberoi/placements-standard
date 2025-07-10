
# Describing a `Placement`: Specification

|Category|Field name|Cardinality|Data Type & Format|Description & Reasoning|
|--------|----------|-----------|------------------|-----------------------|
_Identifying the child_
|| `Child ID` | 1(MUST)|integer|This is the description|
|| `Local Identifier`| 0,1| String | **This** is the description |
||`Is this a planned emergency home search?`|1(MUST)|Boolean| Enter description here|
||`Latest date for placement to start by`​|	1(MUST)|	date|Enter description here|
||`Number of sublings to place with` | | | |
_Location(s) of search_
||`Preferred location for home search `| 	1(MUST)	|string| Enter description here|
||`Primary family location (postcode sector - e.g. GL71)`|	0,1|	string|Enter description here|
||`Is it recommended to find a home close to the primary family location?`|	0,1|	Boolean|Enter description here|
||`Does child go to school currently?`|	0,1|	Categorical|Enter description here|
||`School location (postcode sector - e.g. GL71)`|	0,1	|String|Enter description here|
||`Does the child need to continue to attend this school?`|	0,1|	Boolean| Enter description here |
||`Are there other location(s) of importance for the child that the child needs to visit regularly?`|	0,1 |	Boolean| Enter description here |
||`Please specify which location `| 	0, MANY|	string| Enter description here |
|| `How often does the child need to go to other location  of importance?` |	0,1 |	Categorical  | Enter description here |
|| `Are there any locations to avoid?​ `|	0,1	| Categorical | Enter description here |
|| `Location(s) to avoid (leave blank if not applicable)` |0, MANY	|string| Enter description here |
_Provision requirement_
|| `Communication, language and learning needs` |	1 (MUST) |	Categorical | Enter description here |
|| `Specific communication and language requirements` | 	1, MANY (MUST)| Categorical | Enter description here |
|| `Adaptation to the home` |	1 (MUST) |	Boolean | Enter description here | 
|| `Cultural needs (e.g. place of worship)` | 	1 (MUST)| Categorical | Enter description here | 
_Provision recommendation_
|| `Who can the child be cared for alongside` |	1 (MUST)	| Categorical | Enter description here | 
|| `Can child live with pets/animals?` |	1 (MUST) | Categorical | Enter description here | 
|| `Foster care suitability`| 1 (MUST) |	Categorical | Enter description here |
|| `Foster care suitability `| 1 (MUST) |	Categorical |Enter description here |
|| `Residential suitability`	| 1 (MUST) |	Categorica | Enter description here | 
|| `Supported home suitability` |	1 (MUST) | Categorical | Enter description here | 
||`Minimum adult support ratio	`| 1 (MUST)	|Categorical |  Enter description here | 
_Risk to child_
||`Risk to child: Self-harm`	| 1 (MUST)	|Categorical| Enter description here |
||`Risk to child: Sexual exploitation`	|1 (MUST)	|Cate|gorical|  Enter description here |
||`Risk to child: Criminal exploitation`|	1 (MUST)|Categorical |  Enter description here | 
||`Risk to child: Drug and alcohol use	`|1 (MUST)|	Categorical |  Enter description here |
||`Risk to child: Eating disorder	`|1 (MUST)|	Categorical |  Enter description here |
||`Risk to child: Going missing`	|1 (MUST)	|Categorical |  Enter description here |
||`Risk to child: Other (please specify)`	|0,1|	string |  Enter description here |
_Risk of harm to others or property_
||`Risk to others or property: Physical harm`	|1 (MUST) |	Categorical |  Enter description here |
||`Risk to others or property: Sexual harm`	|1 (MUST)|	Categorical |  Enter description here |
||`Risk to others or property: Fire-setting`	|1 (MUST)|	Categorical |  Enter description here |
||`Risk to others or property: Harm to animals`	|1 (MUST)	|Categorical |  Enter description here | 
||`Risk to others or property: Criminal exploitation	`|1 (MUST)	|Categorical |  Enter description here | 
||`Risk to others or property: Other (please specify)	`|0,1|	string |  Enter description here |
_Additional Support required_
||`Was there any additional provision the home needed to provide to support the child?`|	1(MUST)|	Boolean |  Enter description here | 
||`Additional support (Please specify)`	|0,1 (Conditional MUST)	|Categorical |  Enter description here | 
_Referral Form Information_
||`Name of officer filling referral form`	|0,1|	string |  Enter description here | 
||`Date of referral form filling`	|1(MUST)|	date |  Enter description here |
_Finance Information_
||`Total agreed weekly cost`	|1(MUST)|	integer |  Enter description here |
||`Actual Weekly Cost`	|1(MUST)|	integer |  Enter description here |
_Placement Form Information_
||`Name of officer filling form`	|1(MUST)|	string |  Enter description here | 
||`Date of form filling	`|1(MUST)|date |  Enter description here | 
_Placement information_
||`Placement Location`	|1(MUST)| string |  Enter description here |
||`Provider ID (linked to Ofsted)`	| 1(MUST)|	string |  Enter description here | 
||`Whether Sibling Split Y/N`| 1(MUST)|	Boolean | Enter description here |
||`Placement Type`	| 1(MUST)|	Categorical | Enter description here |
