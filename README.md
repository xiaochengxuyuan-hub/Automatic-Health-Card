# HealthInfoAutoReport

## Two ways

**CAUTION: First, u need post u tmp least 1 time.**

### Through Remote Environment: Github Actions

1. star and fork this repo.
2. set your own those 2 Actions secrets: NUM, PWD
3. commit anything or wait actions auto run.

### Through Local Environment: Python 3.6+

```powershell
pip install requests
pip install beautifulsoup4
pip install lxml
```

Run this:

```powershell
python actions.py account pwd
```
