# About this repository
This is a public repository providing an example of basic Exploratory Data Analysis (EDA) using R and [RStudio](https://www.rstudio.com). After loading a dataset, EDA is often the next steps of data analysis. The basic idea of EDA is to quickly analyse and investigate data sets and summarize their main characteristics, often employing data visualization methods. As presented by IBM, EDA helps 

> "data scientists to discover patterns, spot anomalies, test a hypothesis, or check assumptions. EDA is primarily used to see what data can reveal beyond the formal modeling or  hypothesis testing task and provides a provides a better understanding of data set variables and the relationships between them. It can also help determine if the statistical techniques you are considering for data analysis are appropriate. The main purpose of EDA is to help look at data before making any assumptions. It can help identify obvious errors, as well as better understand patterns within the data, detect outliers or anomalous events, find interesting relations among the variables. "[^EDA]

[^EDA]: IBM (2021) Exploratory Data Analysis. Available at: https://www.ibm.com/cloud/learn/exploratory-data-analysis.


## Steps for basic EDA from scratch

1. Install R (see: https://cran.r-project.org/) and RStudio (see https://www.rstudio.com) in your laptop/desktop.
2. Install the tidyverse package for data manipulation by typing install.packages("tidyverse") . This is required for the step 9.
3. Use some raw dataset in any format you prefer such as CSV (comma-separated values) or XLSX. You may download data any free dataset listed at https://r-dir.com/reference/datasets.html, https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/00Index.html or connect to the World Bank Development Indicators as shown here https://www.r-project.org/nosvn/pandoc/WDI.html. You may also connect to a remote or local database such as MySQL or MongoDB, if you prefer. R is very flexible in terms of connections to data sources.
4. Load the dataset as a data frame and give it a clear and short name (e.g. `povertydata`). We recommend to use a clear convention for names, such as only lower case or camel case (see: https://en.wikipedia.org/wiki/Camel_case).
5. Visualise the dataset by typing: `View(povertydata)` in the R console.
6. Do some basic EDA (exploratory data analysis) of your dataset as shown here https://blog.datascienceheroes.com/exploratory-data-analysis-in-r-intro/ and https://www.r-bloggers.com/2018/11/explore-your-dataset-in-r/.
7. Install the [DataExplorer package](https://www.rdocumentation.org/packages/DataExplorer/versions/0.8.2) (simply typing this in the R console: `install.packages("DataExplorer")`) and run `DataExplorer::create_report(povertydata)`.
