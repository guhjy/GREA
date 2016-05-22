<!-- README.md is generated from README.Rmd. Please edit that file -->
![](logo.png)

### What is 'GREA'?

GREA (Gotta Read 'Em All) is an RStudio Add-In assisting to read all popular file formats into R. In the beginning, the user selects a file on his computer. After proper parsing (which is done interactively), the parsed dataset is assigned to the R working space, with an object name that can be specified by the user. Right now, the following files can be read: .dta, .sav, .mat, .raw, .csv, .txt, .asc, .dat, .xls, .xlsx.

Click [here](http://imgur.com/a/a9M1p) for an interactive comic on why GREA is important.

### News

16.05.2015 - First version of GREA was wrapped up into a package 22.05.2015 - `shiny::fileInput` dependency replaced with `fileChoose()` function

### Installation

To install the Add-In, run the following code:

``` r
devtools::install_github("Stan125/GREA")
```

### Usage

#### 0. Starting the Add-In

Calling the Add-In is simple: just click on the Add-In Tab and select 'Gotta Read Em All'. The Add-In itself quickly pops up and you are good to go!

#### 1. Selecting the dataset

Once the Add-In is started up, press the "choose file" button to select a file on your computer. Then, type in a name for your desired dataset. Once the file is loaded into the Add-In, you may see additional options for parsing the file on the right. Ignore those for now and head right to the "previews" tab.

![Step 1.](step1.png)

#### 2. Looking at the preview

The previews tab shows a preview of what your dataframe would look like if you parsed it with the current settings. If something looks odd (e.g. your column names fell into the first row of the dataset), head back to the first tab. If everything is right, still head back to the first tab.

![Step 2.](step2.png)

#### 3. Adjusting stuff

If the preview of your dataframe looked off, you now have the chance to adjust some parameters (e.g. Sheet Index for Excel files, or separator for .csv files). Adjust them so your preview looks exactly like you want them to. When you are finished and typed in a name for your newly aquired dataset, press "done". Afterwards, the parsed file is assigned to your working space. Boom! You are good to go now.

### Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CONDUCT.md). By participating in this project you agree to abide by its terms.
