# course-ds-base

## Preparation

### 1. Fork / Clone this repository

```bash
git clone https://github.com/iterative/course-ds-base.git
cd course-ds-base
```


### 2. Create and activate virtual environment

Create virtual environment named `dvc-venv` (you may use other name)
```bash
#  use python for windows, python3 for mac and linux
python -m venv dvc-venv

# for linux or mac
python3 -m venv dvc-venv

# Try these if doesn't work (did not worked)
echo "export PYTHONPATH=$PWD" >> dvc-venv/bin/activate
source dvc-venv/bin/activate

powershell -ExecutionPolicy Bypass -File dvc-venv/Scripts/Activate.ps1

# Go to powershell admin (worked)
Set-ExecutionPolicy AllSigned
# to deactivate venv
deactivate

```
Install python libraries

```bash
pip install --upgrade pip setuptools wheel
pip install -r requirements.txt

py -m pip install --upgrade pip setuptools wheel --no-cache-dir
py -m pip install -r requirements.txt --no-cache-dir
```

Add Virtual Environment to Jupyter Notebook

```bash
python -m ipykernel install --user --name=dvc-venv
``` 

Configure ToC for jupyter notebook (optional)

```bash
jupyter contrib nbextension install --user
jupyter nbextension enable toc2/main
```

## 3. Run Jupyter Notebook

```bash
jupyter notebook
jupyter-lab --no-browser --port=2005 --ip=0.0.0.0

```

