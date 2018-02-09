# CS 697 presentation

[![pipeline status](https://git.dbogatov.org/bu/CS-697/badges/master/pipeline.svg)](https://git.dbogatov.org/bu/CS-697/commits/master)

## About this presentation

This presentation is developed by Dmytro Bogatov (dmytro@bu.edu) BU CS PhD student 23'.

The up-to-date version is built in CI and resides as artifact [here](https://git.dbogatov.org/bu/CS-697/-/jobs/artifacts/master/raw/presentation.pdf?job=artifacts) or browse all artifacts [here](https://git.dbogatov.org/bu/CS-697/-/jobs/artifacts/master/browse?job=artifacts).

Presentation is written in LaTeX using beamer package.
It is compile in CI system (Gitlab CI) which checks spelling, lints latex code, verifies `bibfile.bib` and complies source to PDF file (see [.gitlab-ci.yml](.gitlab-ci.yml)).

Main repo is [git.dbogatov.org/bu/CS-697](https://git.dbogatov.org/bu/CS-697).

## How to compile

Prerequisites
* Modern TeX distribution (2016 and later)
	* biber
	* xelatex
* Fira Sans font (https://github.com/carrois/Fira)
* bash 4 (and later)

Or, use `dbogatov/docker-images:latex-latest` docker image.

	# just presentation
	./build.sh

	# presentation with notes
	./build.sh -n on -j presentation-with-notes

	# just bibliography
	./build.sh -b

Output files are in `./dist/`.

### Legal

This work is licensed under **Creative Commons Attribution-NoDerivatives 4.0 International**.
See [LICENSE](LICENSE).
