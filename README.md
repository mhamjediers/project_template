Good Enough Project
====================

A cookiecutter project structure based on the [Reproducible Science Cookiecutter](https://github.com/mkrapp/cookiecutter-reproducible-science) template by [Mario Krapp](https://github.com/mkrapp), and with close resemblances to the philosophy of [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science): *A logical, reasonably standardized, but flexible project structure for doing and sharing data science work.*

Requirements
------------
Install `cookiecutter` command line: `pip install cookiecutter`    

Usage
-----
To start a new science project:

`cookiecutter gh:bvreede/good-enough-project`

Project Structure
-----------------

```
.
├── LICENSE.md
├── README.md
├── config             <- Configuration files
├── data
│   ├── temp           <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
├── docs               <- Documentation, e.g. notebooks for users
├── reports            <- For a manuscript source, e.g., LaTeX, Markdown, etc., or any project reports
│   └── figures        <- Figures for the manuscript or reports
└── src                <- Source code for this project
    |-- external       <- Any external source code, e.g., pull other git projects, or external libraries
```


License
-------
This project is licensed under the terms of the [BSD License](/LICENSE)
