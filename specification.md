
# Describing a `Placement`: Specification

|Category |Field name|Options|Cardinality|Data Type & Format|Description & Reasoning|
|--------|----------|-------|-----------|------------------|-----------------------|
|_Identifying the child_||||| **We suggest that all fields other that 'child ID' which help identify the child, or describe their placement or service history which are already collected universally and in a standardised form are extracted from the case management systems and automatically matched with this new data to minimise the burden placed on placement officers.** |
|| `Child ID` |*ID no.*| 1(MUST)|integer||
|| `Local Identifier`| *free text* | 0,1| String ||
||`Is this a planned emergency home search?`|*Planned/Emergency*|1(MUST)|Boolean||
||`Latest date for placement to start by`​|*date*|1(MUST)|	date||
||`Number of sublings to place with` |*number*| |integer | |
|_Location(s) of search_||||| **The propoed location fields allow a more definition of 'preferred' location, all factors considered, enabling more detailed analysis of the difference between 'ideal' and actual placement locations.**|
||`Preferred location for home search `| *free text* | 	1(MUST)	|string||
||`Primary family location (postcode sector - e.g. GL71)`| *postcode* |	0,1|	string||
||`Is it recommended to find a home close to the primary family location?`| *Y/N* |	0,1|	Boolean||
||`Does child go to school currently?`| *Y/N/NA* |	0,1|	Categorical||
||`School location (postcode sector - e.g. GL71)`| *postcode* | 0,1	|String||
||`Does the child need to continue to attend this school?`| *Y/N* |	0,1| 	Boolean||
||`Are there other location(s) of importance for the child that the child needs to visit regularly?`| Y/N |	0,1 |	Boolean||
||`Please specify which location `| *free text* |	0, MANY|	string||
|| `How often does the child need to go to other location  of importance?` | *daily, few times a week, weekly, every two weeks, monthly, other* |	0,1 |	Categorical  ||
|| `Are you aware of any locations to avoid?​ `| *Y/N*|	0,1	| Categorical ||
|| `Location(s) to avoid (leave blank if not applicable)`|*free text* |0, MANY	|string||
|_Provision requirement_||||| **These fields describe the requirements of the preferred provision. They reflect a focus on how providers conceptualise need, and in particular how this translates into a decision as to whether or not to offer an available placement and at what price all other things being equal. That is not the only way of thinking about needs, but it is the lens which is most appropriate to market analysis because it is how ‘needs’ translate into placements being available or unavailable, and more or less expensive. Together, these fields allows for analysis of relationship between provision requirements and placement outcome and cost.** |
|| `Communication, language and learning needs` | *Y/N/Not Specified* |	1 (MUST) |	Categorical ||
|| `Specific communication and language requirements` | *ESOL, BSL, Makaton, Other, None*| 	1, MANY (MUST)| Categorical ||
|| `Adaptation to the home` |	*Y/N* | 1 (MUST)	|Boolean || 
|| `Cultural needs (e.g. place of worship)` | *Required, Not required, Not Yet Known*  |	1 (MUST)| Categorical || 
|_Provision recommendation_|||||**This section described the preferred provision recommendation. As above, these fields reflect a focus on how providers conceptualise need, and in particular how this translates into a decision as to whether or not to offer an available placement and at what price all other things being equal. That is not the only way of thinking about needs, but it is the lens which is most appropriate to market analysis because it is how ‘needs’ translate into placements being available or unavailable, and more or less expensive. These fields allow comparison of preferred and actual placement and the relationship between provision recommendations and placement outcome and cost.** |
|| `Who can the child be cared for alongside` | *Solo placement recommended, With other children recommended, Only with other older children, Only with other younger children, No preference* |	1 (MUST)	| Categorical || 
|| `Can child live with pets/animals?` | *Y/N/ Don't know*|	1 (MUST) | Categorical || 
|| `Foster care suitability`|*Preferred, Suitable but not preferred, Unsuitable, Not specified* | 1 (MUST) |	Categorical | |
|| `Residential suitability`	|*Preferred, Suitable but not preferred, Unsuitable, Not specified*  | 1 (MUST) |	Categorica | | 
|| `Supported home suitability` | *Preferred, Suitable but not preferred, Unsuitable, Not specified*|	1 (MUST) | Categorical | | 
||`Minimum adult support ratio	`|*[adult:child ratio], 1:1, 2:1, >2:1, Standard ratio, Not specified, Not applicable*| 1 (MUST)	|Categorical | | 
|_Risk to child_|||||**This section describes risks to the child. As above, these fields reflect a focus on how providers conceptualise need, and in particular how this translates into a decision as to whether or not to offer an available placement and at what price all other things being equal. That is not the only way of thinking about risks needs, but it is the lens which is most appropriate to market analysis because it is how ‘needs’ translate into placements being available or unavailable, and more or less expensive. These fields allow analysis of relationship between known risks to the child and placement outcome and cost.** |
||`Risk to child: Self-harm`	|*No known risk, Low risk, High risk* |1 (MUST)	|Categorical| |
||`Risk to child: Sexual exploitation`	| *No known risk, Low risk, High risk* |1 (MUST)	|Categorical| |
||`Risk to child: Criminal exploitation`| *No known risk, Low risk, High risk* |	1 (MUST)|Categorical | | 
||`Risk to child: Drug and alcohol use	`| *No known risk, Low risk, High risk* | 1 (MUST)|	Categorical | |
||`Risk to child: Eating disorder	`| *No known risk, Low risk, High risk* | 1 (MUST)|	Categorical | |
||`Risk to child: Going missing`	| *No known risk, Low risk, High risk* | 1 (MUST)	|Categorical | |
||`Risk to child: Other (please specify)`	| *free text* |0,1|	string | |
|_Risk of harm to others or property_|||||**This section describes risks of harm to others or property assocaited with the referral. As above, these fields reflect a focus on how providers conceptualise need, and in particular how this translates into a decision as to whether or not to offer an available placement and at what price all other things being equal. That is not the only way of thinking about risks or needs, but it is the lens which is most appropriate to market analysis because it is how ‘needs’ translate into placements being available or unavailable, and more or less expensive. These fields allow analysis of relationship between known risks to the child and placement outcome and cost.** |
||`Risk to others or property: Physical harm`	| *No known risk, Low risk, High risk* |1 (MUST) |	Categorical | |
||`Risk to others or property: Sexual harm`	| *No known risk, Low risk, High risk* |1 (MUST)|	Categorical | |
||`Risk to others or property: Fire-setting`	| *No known risk, Low risk, High risk* |1 (MUST)|	Categorical | |
||`Risk to others or property: Harm to animals`	| *No known risk, Low risk, High risk* | 1 (MUST)	|Categorical | | 
||`Risk to others or property: Criminal exploitation	`| *No known risk, Low risk, High risk*| 1 (MUST)	|Categorical | | 
||`Risk to others or property: Other (please specify)	`| *free text* |0,1| 	string | |
|_Additional Support required_|||||**This section describes the additional support required once the actual placement was identified and agreed.  These fields allow analysis of the relationship between support requirements and placement cost** |
||`Was there any additional provision the home needed to provide to support the child?`|*Y/N*|	1(MUST)|	Boolean | | 
||`Additional support (Please specify)`	| *additional supervision, therapeutic support, a worker for respite, taxis to school, other (please specify)* |0,1 (Conditional MUST)	|Categorical | | 
_Referral Form Information_
||`Name of officer filling referral form` | *free text*	|0,1|	string |  | 
||`Date of referral form filling`	| *date* |1(MUST)|	date | |
|_Finance Information_|||||
||`Total agreed weekly cost`	|*number*|1(MUST)|	integer | |
|_Placement Form Information_|||||
||`Name of officer filling form`	| *free text* |1(MUST)|	string | | 
||`Date of form filling	`|*date* | 1(MUST)|date | | 
|_Placement information_||||Enter description here|
||`Placement Location`	|*free text* |1(MUST)| string || 
||`Provider ID (linked to Ofsted)`	| *free text*| 1(MUST)|	string | | 
||`Whether Sibling Split` |Y/N| 1(MUST)|	Boolean | |
||`Placement Type`	| *Residential, Foster, Supported Accomodation* |1(MUST)| 	Categorical | |
