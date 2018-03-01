### Assignment 5

This is assignment 5 for MSDS 6306.

Variables overview, starting from the top...

* `raw_2016` is the raw data pulled from `yob2016.txt`.
* `finder` is a place to store the `grep` string used to locate the errant name.
* `y2016` contains `raw_2016` with the bad data pulled out.

* `raw_2015` is the raw data pulled from `yob2015.txt`.
* `y2015` is just a rename of `raw_2015`, with changed column names.
* `final` contains the merge of `y2016` and `y2015`. We then rip out the additional "gender" column, and make sure we don't have any NAs floating around.
* `totalPopulars` is the sum of the `Total` column that was added to `final`.
* `finalLook` is `final` but arranged by order of occurrences, ascending (so least on top, most on bottom).
* `finalLookFemale` is `finalLook` but with all instances where "gender" = "M" removed.
* `topTen` is the last 10 entries of `finalLookFemale`.

This data is then put into the `pop_girl_baby_names.csv` file.
