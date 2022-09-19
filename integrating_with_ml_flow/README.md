# Experimenting BentoML

## Creating environment to test
```bash
(conda create --name ds_kernel python=3.9 -y) && (conda activate ds_kernel) && (pip install bentoml sklearn jupyterlab)
```

## Running Jupyter lab
```bash
jupyter-lab --NotebookApp.token='' --NotebookApp.password=''
```
