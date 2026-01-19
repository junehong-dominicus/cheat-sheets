**A virtual environment is a self-contained, isolated directory for a project that includes its own Python interpreter and libraries. 

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

## uv
An extremely fast Python package installer and resolver, written in Rust.
### Install uv
```pip install uv```
### Create a virtual environment
```uv venv```
### Install a package
```uv pip install <package_name>```
### Lock dependencies
```uv pip compile requirements.in -o requirements.txt```
### Sync environment
```uv pip sync requirements.txt```

## Conda
### 1. Create a new environment: 
```conda create --name datasci_project python=3.10 pandas numpy matplotlib```
### 2. Activate the environment: 
```conda activate datasci_project```
### 3. List all of your existing conda environments:
```conda env list```
### 4. Deactivate the environment: 
```conda deactivate```

## Docker
### 1. Build an image:
```docker build -t my-image-name .```
### 2. Run a container:
```docker run -p 80:80 my-image-name```
### 3. List running containers:
```docker ps```
### 4. List all containers (running and stopped):
```docker ps -a```
### 5. Stop a running container:
```docker stop <container-id-or-name>```
### 6. Remove a stopped container:
```docker rm <container-id-or-name>```
### 7. List images:
```docker images```
### 8. Remove an image:
```docker rmi <image-id-or-name>```
### 9. Execute a command in a running container:
```docker exec -it <container-id-or-name> bash```
### 10. View container logs:
```docker logs <container-id-or-name>```
### 11. Pull an image:
```docker pull <image-name>:<tag>```
### 12. Run an image:
```docker run <image-name>:<tag>```
### 13. Push an image:
```docker push <image-name>:<tag>```
### 14. Docker Compose
```yaml
version: '3.8'
services:
  web:
    build: .
    ports:
      - "80:80"
    volumes:
      - .:/app
    command: python app.py
```
### 15. Run Docker Compose:
```docker-compose up -d```
### 16. Stop Docker Compose:
```docker-compose down```




**