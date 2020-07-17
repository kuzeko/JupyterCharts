# JupyterCharts

A sample repository with notebook to automatically plot charts from experiments


## To RUN

```
docker run --rm -p 8888:8888 \
        -e JUPYTER_ENABLE_LAB=yes \
        -v "$PWD/notebook":/home/jovyan/work \
        jupyter/datascience-notebook
```


## To publish on GitHub see

https://docs.github.com/en/github/managing-files-in-a-repository/working-with-jupyter-notebook-files-on-github



```
docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes \
        -v "$PWD/notebook":/home/jovyan \
        jupyter/datascience-notebook \
        jupyter nbconvert --to html /home/jovyan/example/charts.ipynb
```
