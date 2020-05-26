# Python Example - Jenkins Workshop

This repository contains example projects for the Jenkins Workshop.

* Run unit test
* Launch Sonar Scan
* Build Docker Image


## Run Test
```
pip3 install pytest
pip3 install pytest-cov
pytest --cov-report xml --cov='.'
```