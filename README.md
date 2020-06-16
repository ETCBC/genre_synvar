# Genre Labels from Syntactic Variation Project

This repository contains genre data from the syntactic variation project. 
The authors of the data are Dirk Bakker, Janet Dyk, Marianne Kaajan, Martijn
Naaijer, and Wido van Peursen. 

Martijn Naaijer has provided the dataset in his [Phd repository](https://github.com/MartijnNaaijer/phdthesis)
as an excel file: https://github.com/MartijnNaaijer/phdthesis/blob/master/Various/subgenres_synvar.xls

That spreadsheet, which is not machine readable, was manually converted into a .csv spreadsheet 
where the genres were split into ranges of book, chapter, and verses 
(see [genre_ranges.csv](genre_ranges.csv)). The ranges are then matched with their appropriate 
BHSA verse nodes and exported as a TF resource under [tf](tf).