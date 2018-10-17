[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/DevStarSJ/Docker-Jupyter_ML/blob/master/LICENSE)

# Docker-Jupyter_ML
Docker Image for Jupyter Notebook include Keras, Scikit-learn, XGBoost, CatBoost, LightGBM


## Shell command for run Jupyter Notebook
```shell
docker run -it -p :8888:8888 conda-ml:latest
```

and connect `http://localhost:8888`

## Run notebook file on docker image
```docker
RUN jupyter nbconvert --execute notebook/[YOUR NOTEBOOK FILE].ipynb --ExecutePreprocessor.timeout=-1 --to markdown --stdout
```