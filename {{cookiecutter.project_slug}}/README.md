# {{cookiecutter.project_name}}

Version {{cookiecutter.project_version}}

{{cookiecutter.project_short_description}}


## Project organization

```
.
├── .gitignore
├── CITATION.md
├── LICENSE.md
├── README.md
├── bin                <- Compiled and external code, ignored by git (PG)
│   └── external       <- Any external source code, e.g., pull from other git projects, or external libraries; ignored by git (RO)
├── config             <- Configuration files (HW)
├── data               <- All project data, ignored by git
│   ├── processed      <- The final, canonical data sets for modeling. (PG)
│   ├── raw            <- The original, immutable data dump. (RO)
│   └── temp           <- Intermediate data that has been transformed. (PG)
├── docs               <- Documentation notebook for users (HW)
│   ├── reports        <- Other project reports and notebooks (e.g. Jupyter notebook, Rmarkdown) (HW)
│   └── manuscript     <- Manuscript source, e.g., LaTeX, Markdown, etc. (HW)
├── results
│   ├── figures        <- Figures for the manuscript or reports (PG)
│   └── output         <- Other output for the manuscript or reports (PG)
└── src                <- Source code for this project (HW)

```


## License

This project is licensed under the terms of the [MIT License](/LICENSE.md)

## Citation

Please [cite this project as described here](/CITATION.md).
