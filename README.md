# Genre Labels from Syntactic Variation Project

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3897469.svg)](https://doi.org/10.5281/zenodo.3897469)

This repository contains genre data as a .csv and as a Text-Fabric file. 
[genre_ranges.csv](genre_ranges.csv) contains ranges of verses which correspond to consecutive chunks of genre.
Both the start and end of the ranges are inclusive, i.e. part of the range.
[verse2genre.csv](verse2genre.csv) contains a simple verse label to genre mapping.

The [Text-Fabric file](tf/c/genre.tf) contains verse node to genre mappings for use with
the [BHSA corpus](https://github.com/ETCBC/bhsa) in [Text-Fabric](https://github.com/annotation/text-fabric).

The authors of the data are Dirk Bakker, Marianne Kaajan, Martijn Naaijer, Wido van Peursen, and Janet Dyk. 
The data was produced in the course of the NWO-funded research project (2013-2018) on syntactic variation
in the Hebrew Bible.

Martijn Naaijer has provided the original dataset in his [Phd repository](https://github.com/MartijnNaaijer/phdthesis)
as an excel file: https://github.com/MartijnNaaijer/phdthesis/blob/master/Various/subgenres_synvar.xls

That spreadsheet, which is not machine readable, was manually converted into the genre_ranges.csv.
The ranges are checked and matched with their appropriate BHSA verse nodes in [ranges2tf.ipynb](ranges2tf.ipynb)

### Genre values

The following values are tagged:

```
prose
poetry
prophetic
instruction
list
```

### Tagging methodology

We use three basic categories: prose, poetry and prophecy for complete books. For example, Genesis is prose, Psalms is poetry, Isaiah is prophecy, etc. The labels are not based on formal criteria, but are intended ot be coarse-grained, intuitive classifications, similar to what one might find in exegetical studies. 

Within prose, we added `list`. These are generally lists of people names. We also added `instruction`, which is a general tag for (mainly) law texts. Finally, we changed `prose` to `poetry` for pieces of poetry emmbedded in prose, such as in Genesis 49.

### TF version

Only version c is exported here, but since the verses do not change from version to version,
you can use `genre.tf` with any version of BHSA.
