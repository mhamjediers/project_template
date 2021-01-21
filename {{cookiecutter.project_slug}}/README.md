# {{cookiecutter.project_name}}

_Version {{cookiecutter.version}}_

{{cookiecutter.project_short_description}}


## Project organization

```
.
├── .gitignore
├── environment.yml
├── LICENSE.md
├── Makefile
├── README.md
├── analysis           <- All project analysis steps
│   ├── out		       <- Final data sets for modeling. (PG)
│   ├── data           <- The original, immutable data dump (RO)
│   ├── temp           <- Intermediate, transformed data (PG)
│   ├── results        <- Figures, Tables and other output for manuscript (PG)
│	└── jobs		   <- Analysis scitps (HW)
├── latex              <- Manuscript source (HW)
├── literature		   <- Some literature specific to this project
├── presentation	   <- Source for presentations (HW)
└── submission		   <- Finalized submissions (HW)

```
*RO* = read-only, *HW* = human-writeable, *PG* = project-generated. Repository organization implemented with [cookiecutter](https://github.com/cookiecutter/cookiecutter) using an adapted version of the [good-enough-project template](https://github.com/bvreede/good-enough-project) by Barbara Vreede. The fork is available [here](https://github.com/maximilian-sprengholz/good-enough-project).

## Usage

To replicate the analysis and docs, you need to have [Anaconda](https://www.anaconda.com/products/individual) installed and `conda` available via shell. Windows users probably need [Make](https://www.gnu.org/software/make/) too. Do the following in your shell:

```bash
# create and activate conda environment (initialized as subdirectory ./env)
cd /path/to/{{cookiecutter.project_slug}}
conda env create --prefix ./env --file environment.yml
conda activate ./env
# check if environment is active and python is in it
make checksetup
# run analysis and make docs
make all
```

## License

This project is licensed under the terms of the [MIT License](/LICENSE.md)

## Citation

Please cite this project as:

{{ cookiecutter.full_name }} ({% now 'local', '%Y' %}). {{cookiecutter.project_name}}, version {{cookiecutter.version}}. Url: {{cookiecutter.git_url}}/{{cookiecutter.git_username}}/{{cookiecutter.project_slug}}
