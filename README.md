# Practica 5: XAI - Partial Dependence Plots

Este repositorio contiene la solucion de la practica de metodos model-agnostic
con Partial Dependence Plots (PDP).

## Contenido

- `XAI3.pdf`: enunciado original.
- `day.csv` y `hour.csv`: datos de alquiler de bicicletas.
- `kc_house_data.csv`: datos de precios de viviendas.
- `Practica5_PDP.Rmd`: informe reproducible en R Markdown.
- `Practica5_PDP.pdf`: informe final generado.

## Requisitos

La practica esta preparada para ejecutarse con R 4.4.2. En este equipo R esta en:

```powershell
C:\Program Files\R\R-4.4.2\bin\Rscript.exe
```

Paquetes usados:

- `readr`
- `dplyr`
- `ggplot2`
- `randomForest`
- `gridExtra`
- `viridis`
- `rmarkdown`
- `knitr`

No se usa el paquete `pdp`; los PDP se calculan manualmente.

## Como generar el informe

Desde esta carpeta:

```powershell
$env:RSTUDIO_PANDOC='C:\Program Files\RStudio\resources\app\bin\quarto\bin\tools'
& 'C:\Program Files\R\R-4.4.2\bin\Rscript.exe' -e "rmarkdown::render('Practica5_PDP.Rmd', output_format='pdf_document')"
```

El resultado es `Practica5_PDP.pdf`.

## Entrega

El entregable pedido por el enunciado es el enlace al repositorio de GitHub que
contiene los datos, el codigo reproducible y el informe final en PDF.
