# ProjectScript

Full description on how the code script was built.

# Preliminaries

_Working in R Studio from here on_

Load packages

```r
library("data.table")
library("reshape2")
```

Set path

```r
path <- getwd()
```

# Get the data

Download

```r
url <- "https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip"
f <- "Dataset.zip"
if (!file.exists(path)) {
    dir.create(path)
}
download.file(url, file.path(path, f))
```
