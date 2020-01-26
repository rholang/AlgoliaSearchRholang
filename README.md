# DocSearch scraper

This repository holds the code of the DocSearch scraper used to power the hosted
version of DocSearch. DocSearch scaper is used as search for the [rholang/rholang.github.io](rholang/rholang.github.io) implementation.

## Pre-requisites

- Install Python 3.6. Only this version have no error messages displayed (check that environment variables for python are set).
- Install pipenv
  - run command line with admin rights
  - pip install pipenv

## Setup project

- Open this project with vscode -> cd into /DocSearch-Srapper
- pipenv install --dev
- rename .env.example to .env

## Folder structure

- .evn

  - you need the keys from algolia and the chromedriver path
    - change APPLICATION_ID, API_KEY to yours from algolia
    - change CHROMEDRIVER_PATH to your path (in folder chromedriver_win32)

- config/website.json
  - config, what css selector to parse on your website

## Start scrapping

- pipenv run python ./docsearch run ./configs/website.json
