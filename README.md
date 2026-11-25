# Freight Audit Pipeline #

## PREREQUISITE

- Git
- Python 3.12.10
- PowerShell
- Internet access to download packages and hook dependencies

## Setup

Run these commands in PowerShell:

```powershell
git clone https://github.com/Arfat-khalid/freight-audit.git freight_audit
cd freight_audit

# Verify the Python version
python --version

# Create and activate the virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# Install dependencies

.\.venv\Scripts\python.exe -m pip install --upgrade pip
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe -m pip check

.\.venv\Scripts\pre-commit.exe install
.\.venv\Scripts\pre-commit.exe run --all-files

.\.venv\Scripts\dbt.exe debug --project-dir dbt --profiles-dir dbt
.\.venv\Scripts\dbt.exe build --project-dir dbt --profiles-dir dbt
```

## OVERVIEW

_To be added_

## ARCHITECTURE

_To be added_


## PREREQUISITES

_To be added_

## SETUP

_To be added_


## RESULTS

_To be added_
