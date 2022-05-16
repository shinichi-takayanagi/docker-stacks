## What's this
Japanese NLP notebook.

## Build
```
docker build -t japanese-nlp-notebook .
```

## Launch JupyterLab
```
docker run --rm \
    -p 8888:8888 \
    -e JUPYTER_ENABLE_LAB=yes \
    -v $(pwd):/home/jovyan/work/ japanese-nlp-notebook
```
