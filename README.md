# RINSE - Registry of non-native species in the Two Seas region countries (Great Britain, France, Belgium and the Netherlands)

## Rationale

This repository contains the functionality to standardize the data of [Zieritz et al. (2014)](https://doi.org/10.3897/neobiota.23.5665) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). It was developed for the [TrIAS project](http://trias-project.be).

## Workflow

[source data](https://github.com/trias-project/rinse-registry-checklist/blob/master/data/raw/oo_30975.xlsx) (downloaded as [Supplementary Material 1](http://neobiota.pensoft.net//lib/ajax_srv/article_elements_srv.php?action=download_suppl_file&instance_id=31&article_id=4007)) → Darwin Core [mapping script](http://trias-project.github.io/rinse-registry-checklist/dwc_mapping.html) → generated [Darwin Core files](https://github.com/trias-project/rinse-registry-checklist/tree/master/data/processed)

## Published datasets

* [Dataset on the IPT](https://ipt.inbo.be/resource?r=rinse-registry-checklist)
* Dataset on GBIF

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md         : Description of this repository
├── LICENSE           : Repository license
├── .gitignore        : Files and directories to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
├── docs              : Repository website GENERATED
│
└── src
    ├── dwc_mapping.Rmd  : Darwin Core mapping script, core functionality of this repository
    └── src.Rproj        : RStudio project file
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_mapping.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `/docs`

## Contributors

[List of contributors](https://github.com/trias-project/rinse-registry-checklist/contributors)

## License

[MIT License](https://github.com/trias-project/rinse-registry-checklist/blob/master/LICENSE)
