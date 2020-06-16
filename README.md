# Genre Labels from Syntactic Variation Project

This repository contains genre data as a .csv and as a Text-Fabric file. 
[genre_ranges.csv](genre_ranges.csv) contains ranges of verses which correspond to consecutive chunks of genre.
Both the start and end of the ranges are inclusive, i.e. part of the range.
The [Text-Fabric](tf/c/genre.tf) file contains verse node to genre mappings for use with
the [BHSA corpus](https://github.com/ETCBC/bhsa) in [Text-Fabric](https://github.com/annotation/text-fabric).

The authors of the data are Dirk Bakker, Marianne Kaajan, Martijn Naaijer, Wido van Peursen, and Janet Dyk. 
The data was produced in the course of the NWO-funded research project (2013-2018) on syntactic variation
in the Hebrew Bible.

Martijn Naaijer has provided the original dataset in his [Phd repository](https://github.com/MartijnNaaijer/phdthesis)
as an excel file: https://github.com/MartijnNaaijer/phdthesis/blob/master/Various/subgenres_synvar.xls

That spreadsheet, which is not machine readable, was manually converted into the genre_ranges.csv.
The ranges are checked andmatched with their appropriate BHSA verse nodes in [ranges2tf.ipynb](ranges2tf.ipynb)

### TF version

Only version c is exported here, but since the verses do not change from version to version,
you can use `genre.tf` with any version of BHSA.
