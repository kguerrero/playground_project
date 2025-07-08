# SETUP

## base environment

```bash

conda create -- name playground_project python=3.13
conda activate playground_project
pip install uv

```
    
## install dependencies

navigate to `playground_project` directory that contains the uv lock file and create vertual environment

```bash

uv sync


```