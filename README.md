# Selecting-rows-from-data-frames-at-random
This video shows you how to  1. Select random rows from observations with and without replacement  2. Remove observations from a data 
### SELECTING  ROWS FROM THE DATAFRAME  AT RANDOM ###
worms<-read.table("worms.txt", header = TRUE)
View(worms)
attach(worms)


# selecting 10 ramdom rows of the 20 observations  without repacement (default)
worms[sample(1:20, 10), ]
# Another way 
worms[sample(1:20, 10, replace = FALSE), ]

# selecting  14 ramdom rows of the 20 observations  with repacement 
worms[sample(1:20, 14, replace = TRUE), ]

worms[ , -c(1:3)] # remove the first 3 columns 
