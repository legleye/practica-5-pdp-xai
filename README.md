# Practice 5: XAI - Partial Dependence Plots

This repository contains the solution for the model-agnostic methods practice
using Partial Dependence Plots (PDP).

## Contents

- `XAI3.pdf`: original assignment statement.
- `day.csv` and `hour.csv`: bike rental data.
- `kc_house_data.csv`: house price data.
- `Practica5_PDP.Rmd`: reproducible report in R Markdown.
- `Practica5_PDP.pdf`: final generated report.

## Requirements

The practice is prepared to run with R 4.4.2. On this computer, R is located at:

```powershell
C:\Program Files\R\R-4.4.2\bin\Rscript.exe
```

Packages used:

- `readr`
- `dplyr`
- `ggplot2`
- `randomForest`
- `gridExtra`
- `viridis`
- `rmarkdown`
- `knitr`

The `pdp` package is not used; the PDP values are computed manually.

## How to Generate the Report

From this folder:

```powershell
$env:RSTUDIO_PANDOC='C:\Program Files\RStudio\resources\app\bin\quarto\bin\tools'
& 'C:\Program Files\R\R-4.4.2\bin\Rscript.exe' -e "rmarkdown::render('Practica5_PDP.Rmd', output_format='pdf_document')"
```

The output is `Practica5_PDP.pdf`.

## Submission

The deliverable requested in the assignment is the GitHub repository link. The
repository contains the data, the reproducible code, and the final PDF report.
