A virtual environment is a self-contained, isolated directory for a project that includes its own Python interpreter and libraries. 

## Python venv
### Step 1: Create the Virtual Environment
``` python -m venv .venv ```
### Step 2: Activate the Virtual Environment 
|Platform|Shell|Command|
|---|---|---|
|macOS/Linux|bash/zsh|``` source .venv/bin/activate ```|
|Windows|Command Prompt|``` .venv\Scripts\activate.bat ```|
|Windows|PowerShell|``` .& .venv\Scripts\Activate.ps1 ```|
### Step 3: Install Packages and Use 
### Step 4: Deactivate the Environment
``` (.venv) $ deactivate ```
### pyenv
The most widely recommended tool for managing multiple Python versions on a single system.

## Conda
### 1. Create a new environment: 
```conda create --name datasci_project python=3.10 pandas numpy matplotlib```
### 2. Activate the environment: 
```conda activate datasci_project```
### 3. Verify installed packages: 
```conda list```
### 4. Deactivate the environment: 
```conda deactivate```




