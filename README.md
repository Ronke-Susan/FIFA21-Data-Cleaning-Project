# FIFA21 DATA CLEANING AND TRANSFORMATION
### OBJECTIVE

The objective of this data cleaning project is to ensure the quality, consistency, and usability of the FIFA 21 player dataset obtained from Kaggle.

### TOOL USED
Python

Libraries: Pandas and Numpy 

### MOTIVATION

The motivation behind this project is to expand and diversify my portfolio by incorporating new and exciting projects. I would like to express gratitude to Danny Ma for providing the idea for this particular project.

### ABOUT THE DATA
The dataset utilized for this data cleaning project in FIFA 21 was acquired from [Kaggle](https://www.kaggle.com/datasets/yagunnersya/fifa-21-messy-raw-dataset-for-cleaning-exploring?select=fifa21_raw_data.csv). It comprised detailed data and statistics pertaining to various players featured in the FIFA 21 video game. The dataset consisted of 18,979 rows and 77 columns.
For individuals who are not well-versed in football terminology, some of the column names might be ambiguous or unclear. To address this, I conducted research and found comprehensive descriptions of these column attributes on these three websites: [Website 1](https://fifauteam.com/fifa-21-attributes-guide/#:~:text=Positioning%20is%20the%20player's%20ability,the%20ball%20in%20dangerous%20areas.) , [Website 2](https://www.fifplay.com/encyclopedia/player-attributes/) and [Website 3](https://www.fifplay.com/fifa-21-player-attributes/). These resources provided in-depth explanations of the attributes associated with the columns.
Furthermore, certain attributes, particularly those represented by abbreviations like DEF, PAS, and others, were explained in [FIFA 22](https://www.fifplay.com/fifa-22-player-attributes/), which provided additional clarity and understanding.

#### Columns Description
Below is a description of each column in the dataset

1. photoUrl - links to the players photographs         
2. LongName - players full names       
3. playerUrl - links to the players websites    
4. Nationality - players countries of origin        
5. Positions - field positions players play on the field   
6. Name - players initials with surnames  
7. Age - players ages
8. OVA - the average of the key player attributes rates of a player within their potential rate calculated based on their position and international reputation.
9. POT - players potential  rated over 100
10. Team & Contract - players current teams and expected period of stay with the teams
11. ID - players identification numbers
12. Height - players heights measured in feet and inches
13. Weight - players weight measured in pounds
14. foot - players preferred foot for playing  
15. BOV  - best overall in percentage
16. BP   - players best position on the field
17. Growth - represents the potential increase in a player's skills and abilities as they progress and gain experience in the game. 
18. Joined - date in which players joined their teams
19. Loan Date End - date when players on loan contracts are terminated 
20. Value(€) - players financial worth in euros
21. Wage(€) - players weekly allowance in euros
22. Release Clause(€) - a predetermined fee in euros under which a player can be transferred to another club.
23. Attacking - a player’s ability to spot open space and move into good positions that offer an attacking advantage
24. Crossing - the player’s accuracy at crossing the ball during both normal running and free kick set pieces.
25. Finishing - the players’ accuracy of shots using foot, inside the penalty area
26. Heading Accuracy - the heading accuracy of the players for either a pass or a short.
27. Short Passing  - players’ accuracy and speed of passing over a short distance
28. Volleys -the accuracy and power of volleys at goal.
29. Skill- the sum total of all skill attributes scores i.e sum of dribbling, curve, FK accuracy, long passing and ball control scores.
30. Dribbling - player’s ability to carry the ball and past an opponent
31. Curve - player’s ability to curve the ball when passing and shooting
32. FK Accuracy - player’s accuracy for taking free kicks
33. Long Passing - classifies how well a player performs a long pass in the air to his teammate.
34. Ball Control - player’s ability to control the ball as he receives it.
35. Movement - the sum total of the players movement attributes scores i.e sum of acceleration, sprint speed, agility, reactions and balance.
36. Acceleration - the increment of a player’s running speed.
37. Sprint Speed  - how fast the player runs while at top speed.
38. Agility -  how agile the player is while moving or turning.
39. Reactions  - how quickly a player responds to a situation happening around him.
40. Balance - players’ ability to maintain balance after a physical challenge.
41. Power - the sum total of the players’ power attributes scores. I.e sum of shot power, jumping, stamina, strength, long shots.
42. Shot Power - the amount of power a player can put into a shot while still keeping it accurate.
43. Jumping - the player’s ability and quality for jumping from the surface for headers.
44. Stamina - the rate at which a player will tire during a game.
45. Strength -  the quality or state of being physically strong.
46. Long Shots - A player’s accuracy for the shots taking from long distances.
47. Mentality - the sum total of aggression, interceptions, positioning, vision and penalties scores.
48. Aggression - the frequency and the aggression of jostling, tackling and slide tackling.
49. Interceptions  - the player’s ability to read the game and intercept passes.
50. Positioning  - the players ability to take up good positions on the field during a game.
51. Vision - the player’s awareness of the position of his teammates & opponents around him.
52. Penalties - the accuracy of shots from inside the penalty area.
53. Composure - distance at which the player with the ball starts feeling the pressure from the opponent.
54. Defending - A player’s ability to defend
55. Marking - A player’s capability to mark opposition player(s).
56. Standing Tackle - the ability of the player to time sliding tackles so that they win the ball rather than give away a foul while on their feet (dispossess an opponent of the ball while standing).
57. Sliding Tackle - the ability of the player to time sliding tackles so that they win the ball rather than give away a foul (dispossess an opponent while sliding).
58. Goalkeeping  -  the sum total of goal keeping attributes scores i.e sum of GK diving, GK handling, GK kicking, GK positioning and GK reflexes.
59. GK Diving  - Goal keeper’s ability to make a save whilst diving through the air.
60. GK Handling - it is the frequency that the keeper catches the ball rather than parrying it and whether or not he holds onto it.
61. GK Kicking  - the goal keeper’s length and accuracy of goal kicks, from out of the hands or on the ground.
62. GK Positioning  - It is the goal keeper’s ability to position himself correctly when saving shots.
63. GK Reflexes - the agility of the goalkeeper when making a save.
64. Total Stats  - the sum of all the numerical ratings assigned to various skills and abilities possessed by the player. The attributes that contribute to the total stats may vary depending on the player's position and playing style.
65. Base Stats - the sum total of PAC, SHO, PAS, DRI, DEF, PHY scores.
66. W/F - short for weak foot, graded out 5 stars refers to player’s ability to control, pass and shoot the ball with his weak foot.
67. SM - short for skill moves, rated out of 5 stars, refers to the skill moves a player ia able to do.
68. A/W  - short for attacking work rate, displayed as low, medium or high. Refers to how much effort a player puts into attacking.
69. D/W  - short for defense work rate,displayed as low, medium or high. Refers to how much effort a player puts into defending.
70. IR - short for international reputation rated out of 5 stars, represents how well-known and respected a player is at the international level.
71. PAC - short for pace,refers to a player’s speed in walking/running.
72. SHO  - short for shooting,refers to a player's general shooting strength and accuracy. it determines finishing skill and shot power.
73. PAS - short for passing, refers to how accurate a player passes the ball to a teammate with vision.
74. DRI - short for dribbling, a player's ability to carry the ball and past an opponent while being in control. It notes ball control, agility and balance.
75. DEF - short for defending(attribute), refers to a player's ability to defend in relation to tackling and marking.
76. PHY - short for physical, refers to a player’s physical and body situation in relation to strength and stamina.
77. Hits - refers to the number of times a player's item or card has been viewed or accessed by users in the FIFA video game. It is used to assess a player's market value or demand within the game  

### DATA QUALITY AND TIDINESS ISSUES
#### Data Quality: The following data quality checks were performed on the data

* Completeness - the fifa21 dataset was checked for completeness. It had a large number of missing values in the ‘Loan Date End’ column. The percentage of missing values in the loan date end column is 94.66%. Hence, the data is not complete
* Validity: Unwanted characters as a result of web scraping impacted the validity of the data. Not all columns were in the right data type
* Accuracy: All information in the dataset are correct and reflect real life situations 
* Consistency: Not all columns in the dataset had consistent entries. For example, the contract_period column (though extracted from the team&contract column) is expected to reflect a time-period from the joined year to the loan date end year like “2010-2015”  but there were entries like “30, Jan 2021”, “Free” within the same column. Another is the “Hit” column that had 1.2K values which implies 1200 in some instances and actual numerical values in other instances.
* Timeliness: just like the name of the data implied, fifa21 contained all information about players up to the year 2021.
* Uniqueness: There was a single occurence of duplicate entries in the dataset
* Integrity: The data is reliable. It was scrapped from a reliable source and contained reliable information

#### Data Tidiness: The following tidiness checks were performed on the data

* Each variable is a column: each variable in the fifa21 dataset is a column  ✔
* Each observation is a row: each observation is a row. Each player is a unique observation ✔
* Each type of observation unit is a table.: There are corresponding columns for every row observation such that they form a table ✔

### DATA CLEANING PROCESS

In no particular order the following data cleaning processes were performed on the dataset.

* Data Transformation: changed the data types of some numerical columns such as Value, Wages and Release Clause stored as strings into floats and “Hits” and “Weight” columns into integers using the astype() function. Converted the “Joined” column into datetime using the pd.to_datetime() function.
* Feature Extraction: Created new columns from existing columns in the dataset. Separated the “Team&Contract” column into “Team” and “Contract_period” columns, converted the “Height” column from feet&inches into centimeters and stored them in a separate column named “Height_cm” , created “Day_joined” and “Month” columns from the “Joined” column
* Handling Inconsistencies: Not all values in “Contract_period” and “Hits” column were in the same format. Inconsistent formats were removed and replaced with the right format. For the “Hits” column, a mathematical function was defined and applied to the column using the apply() and lambda functions to convert values with “K” suffix to thousands.
For the “Contract_period” column, a filtering condition was used to identify values that were not complete time periods i.e instead of having like “2010-2015”, they had only single year values. By comparing the “Joined”,”Loan Date End” and “Contract_period” columns, I was able to identify the missing year values as joined year values and extracted them from the “Joined” column.
* Handling duplicates: searched for duplicates in the data using duplicated() function and set the players’ ID as a subset parameter (since each player has a unique ID). The duplicate row was then deleted using the drop_duplicate() function and setting the keep parameter to first to retain the first occuring observation.
* Removing unwanted characters: Unwanted characters such as currency symbols, stars signifying ratings, newlines, etc were removed from the dataset using the replace() function and setting the regex parameter to True. A dictionary-based replacement was used to replace “M” and “K” values in the “Wages”, “Value” and “Release clause” columns with “e6” and “e3” thereby converting them to their respective millions and thousands before changing their data types
* Handling missing values: The “Loan Date End” column was eventually dropped using the dropna() function after gathering useful information from it especially when deciding how best to fill the contract_period column.


