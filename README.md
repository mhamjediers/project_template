# Project template

_Version 0.1.1_

A cookiecutter project structure based on the [Reproducible Science Cookiecutter](https://github.com/bvreede/good-enough-project) template by [Barbara Vreede](https://github.com/bvreede), and with close resemblances to the philosophy of [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science): *A logical, reasonably standardized, but flexible project structure for doing and sharing data science work.*

The name (and most of the structure) are derived from the paper [Good Enough Practices in Scientific Computing](https://doi.org/10.1371/journal.pcbi.1005510), Wilson _et al._, PLOS Computational Biology (2017).

## Requirements

Install `cookiecutter` on the command line use for conda:

```bash
conda config --add channels conda-forge
conda install cookiecutter
```
For pip:

```bash
pip install cookiecutter
```

## Usage

To start a new science project:

`cookiecutter gh:mhamjediers/project_template`

## Project Structure

The project structure distinguishes three kinds of folders:
- read-only (RO): not edited by either code or researcher
- human-writeable (HW): edited by the researcher only.
- project-generated (PG): folders generated when running the code; these folders can be deleted or emptied and will be completely reconstituted as the project is run.


```
.
├── .gitignore
├── environment.yml
├── LICENSE.md
├── Makefile
├── README.md
├── data               <- All project data, ignored by git
│   ├── processed      <- Final data sets for modeling. (PG)
│   ├── raw            <- The original, immutable data dump (RO)
│   └── temp           <- Intermediate, transformed data (PG)
├── docs               <- Documentation
│   ├── manuscript     <- Manuscript source (HW)
│   └── reports        <- Other project reports and notebooks (HW)
├── results
│   ├── figures        <- Figures for the manuscript or reports (PG)
│   ├── misc           <- Other output (PG)
│   └── tables         <- Tables (PG)
└── src                <- Source code (HW)
    └── external       <- External source code used (RO)

```

The project is adapted to my basic social science workflow that uses [Anaconda](https://www.anaconda.com/products/individual) and the `environment.yml` to create a local environment and [Makefile](https://www.gnu.org/software/make/) to automate stuff.

## License

This project is licensed under the terms of the [MIT License](/LICENSE.md).
