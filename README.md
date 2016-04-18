# L4
Unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip and rename the folder with "data".

Run R script.

Two output files are generated in the current working directory:
  merged_data.txt (7.9 Mb): it contains a data frame called cleanedData with 10299*68 dimension.

   data_with_means.txt (220 Kb): it contains a data frame called result with 180*68 dimension. 


Use data <- read.table("data_with_means.txt") command in RStudio to read the file. this will creat a data frame with 180 rows with all combinations for each of the 66 features.
