# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

v0.1.0 = [Reproducible Science Cookiecutter](https://github.com/bvreede/good-enough-project)

## v0.1.1

Geared toward using Anaconda, cleaned up some clutter unnecessary for smaller (non-machine learning) projects. Re-introduced a Makefile.

### Added
- content:
    - `README.md`
        - citation info
        - usage instructions for conda env
- folders:
    - `results/misc`
    - `results/tables`
    - `src/external`
- files:
    - `environment.yml`
    - `Makefile`

### Removed
- folders:
    - `bin`
    - `config`
    - `results/output`
- files:
    - `requirements.txt`
    - `CITATION.md`
