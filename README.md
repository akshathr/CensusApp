# CensusApp
counties.file = file.choose()
helpers.file = file.choose()
counties = readRDS(counties.file)
head(counties)

library(maps)
library(mapproj)
source(helpers.file)
percent_map(counties$white, "darkgreen", "% White")