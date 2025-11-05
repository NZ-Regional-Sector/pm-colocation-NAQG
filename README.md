# Tools to analyse PM co-location data

## Purpose

Repository of tools and guidance for co-location exercises of air particulate matter monitoring equipment, following discussions between regional councils and industry representatives in New Zealand.

## Usage
1. Put your input data in the `data` folder.
2. "Knit" the "Rmd" file located in the root folder
    1. If using **Rstudio** or **VSCode**
        1. Open the file `pm_colocation_report.Rmd`
        2. Click on the **Knit** button at the top right of the editor panel.
    2. If using a different IDE or text editor
        1. Open an R session in the `R` folder
        2. Give the `knit` command:
        ```
        markdown::render(input = "pm_colocation_report.Rmd")
        ```

The output file will be located in the same folder than the Rmd file. Keep in mind that the `Rmd` file will look for the input `xlsx` file so make sure that the name of your input file matches what's in the header of the `Rmd` file (the `data_path` parameter).
