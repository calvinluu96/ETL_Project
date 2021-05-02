# ETL_Project

## Extract
We gathered data from two datasets found on Kaggle, both were formatted as CSV files. 
The first was Player vs Player (PvP) data collected for the game Pokemon Go, since we could not find any data for the mainline Pokemon games.
The second was a "pokedex" that gives information from Japanese and German names of pokemon to what type of species or pokemon they are and what weaknesses and strengths they have against other pokemon.

## Transform
We first looked at which columns from each of the datasets could be potentially useful, and dropped any columns we thought were not relevant.
Once we had all useful information, we merged the datasets to create one dataframe. We only kept entries where the pokemon were in both the pokedex and the PvP data. This prevented us from dealing with different versions of the same pokemon (such as Mega or regional forms).
We also dropped some columns that we felt were redundant (exist in both datasets)

## Load
We loaded the merged data and sorted by PvP score so we could see which pokemon would be most useful to use in PvP battles, and see what information about each pokemon would be useful, such as their stats or types. 
