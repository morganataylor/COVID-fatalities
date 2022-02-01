# Overview

These subfolders contain all R markdown files (.Rmd) and corresponding html files created for processing the raw data. The output of each markdown is then stored in the corresponding `processed_data` subfolder in the repository. All processed datasets are saved as .rds to preserve all data types and classes, thus avoiding redundant efforts to redefine data types in subsequent markdowns.

# COVID-19 Fatalities: `covid`

There are three publicly available data sources used in this analysis for quantifying the total number of COVID-19 fatalities in the US:

* Centers for Disease Control and Prevention (CDC)
* Johns Hopkins University (JHU)
* New York Times (NYT)

The three sources were chosen not only due to their established reputation as valid COVID-19 data sources but also to capture the variation in reported COVID-19 fatalities. Each source dataset is processed individually, and then the three are combined to create one processed dataset that represents total COVID-19 fatalities.

* `CDC_processing.Rmd` &#8592; `CDC_processed.rds`
* `JHU_processing.Rmd` &#8592; `JHU_processed.rds`
* `NYT_processing.Rmd` &#8592; `NYT_processed.rds`
* `CDC_processed.rds` + `JHU_processed.rds` + `NYT_processed.rds` &#8592; `covid_total_processed.rds`
