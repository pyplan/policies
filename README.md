# ![Pyplan](./docs/images/logo.png)

This site describes Pyplan policies and procedures related to architecture and data security and privacy.


## Requirements

* [python 3](https://www.python.org/downloads/)

## Clone repo

``` bash
cd  [your-projects-path]
git clone https://github.com/pyplan/policies.git
```

## Create venv

``` bash
# Create virtual environment
cd [your-projects-path]/policies
python3 -m venv venv
. venv/bin/activate # in linux/mac os
venv\Scripts\activate.bat # in windows
pip install --upgrade pip
pip install -r requirements.txt
```

## Live preview

``` bash
cd [your-projects-path]/policies
sphinx-autobuild docs docs/_build --port 5500 --open-browser
```


## How to contrib

1. Update local branc **main**.
2. Create a new branch with descriptive name(Ex. schedule-task), from **main** branch.
3. Update/create files .rst/.md, inside the **/docs** folder.
4. Create Pull Request from the new branch to the **main** branch.

