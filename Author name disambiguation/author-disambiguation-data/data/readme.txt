This data set is used for studying name disambiguation in digital library. It contains 110 author names and their disambiguation results (ground truth). Each author name corresponds to a raw file in the "raw-data" folder and an answer file (ground truth) in the "Answer" folder. 

- Raw file: the raw file is formatted as a XML file. In the XML file, the author name is associated with a number of publications. An example of a publication is as follow:
"
  <publication>
		<title>Explanation-based Failure Recovery</title>
		<year>1987</year>
		<authors>Ajay Gupta</authors>
		<jconf>AAAI</jconf>
		<id>13048</id>
		<label>0</label>
		<organization>null</organization>
	</publication>
"	
where <title> denotes the title of the publication; 
<year> denotes the publication year;
<jconf> denotes the publication venue;
<id> denotes the publication id;
<label> denotes the labeled person, e.g., all publications with "<label>0</label>" can be considered as published by the same person;
<organization> denotes the affiliation of the author(s).


- Answer file: the answer file is the ground truth. It is actually extracted from the raw-file by viewing publications with the same "<label>0</label>" as a person. The format is in plain text. The following is an example:
"
#Ajay Gupta
#1:13048 388794 596099 1265282 1179332 675629 39153 258611
#2:988870 1490190
#3:1393934
#4:1398544
#5:1739014
#6:1671104 515636 1678096
#7:1126381 1205032 275987 277587 276300 1549674 1034401
#8:600181 846439 149270 175996 264268 264291 299548 1384744 300057 302056 545651 1212517
#9:1316053
"
where the first line denotes the author name and each of the following line indicates a disambiguate person. For example the first line indicates that an author published 8 papers. The corresponding IDs of those papers are respectively 13048, 388794, 596099, 1265282, 1179332, 675629, 39153, 258611.


