# Some R posibilities

The objective of this project is to show some of the interesting things that you can do with R. 

It is important to start using R with RStudio projects. 
The project is a folder and all the scripts and data for this project should be ordered into this folder. 
This project folder is what you will share when collaborating. 

To open this project press twice on the *TEA_DAA_some-R-posibilities.Rproj* file.

Tip: You can render this file pressing on the "**Preview**" button.

# Repository

This project is available from bitbucket:
https://bitbucket.org/alfonsogar/tea_daa_some-r-posibilities/downloads/

# Scripts

- *01_base-R-plots.R* shows how easy is to make a plot in base R. 

- *02_packages-to-import-export-from-Excel.R* script shows packages to import and export files to and from Excel. Also from/to csv. 

- *03_fancy-plots.R* script shows the plotting power of R package *ggplot2*. Only some easy examples. 

- *04_basic-quarto-document.Rmd* and *.qmd* show the basic structure of Rmd and qmd documents. 

# Protocol

1. Open the project. press twice on the *TEA_DAA_some-R-posibilities.Rproj* file

2. Run the R scripts in order, row by row, clicking Ctl-Enter (or press Run). 

3. Some code might be commented (with an # before) and will not run unless erase the # or select the line without it. This is used for comments and for code shown but not run. 

4. Try to read the code. Do not worry if you do not understand it yet. 

5. Open and render the Rmd document (push *Preview*, *Knit* or *Render* button). Look the new document. Read the code and identify the R chunks from the text. 

6. Upload the project into your github repository (see *Git* chapter). 

7. Try to change things in the code, and use Git to Commit and Push the changes. 

8. Enjoy.

# Git

follow this instructions to upload the project to your github:
https://docs.github.com/en/github/importing-your-projects-to-github/importing-source-code-to-github/adding-an-existing-project-to-github-using-the-command-line

# Other tips

In a project folder should be always a README.md file with the description of the project, a data folder with the data and one or more scripts, usually ordered with numbers in front. 

Example to source (run completely) a specific R file:

```
source("01_base-R-plots.R")
```

Example to render a Rmd file from console:  

```
rmarkdown::render("04_basic-rmarkdown-document.Rmd",
   output_format = "html_document") # html
```

Example to render a quarto file from console:  

```
quarto::quarto_render("04_basic-quarto-document.qmd", 
                   output_format = "html")  # html
```



