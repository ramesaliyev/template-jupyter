# Jupyter Template

## Python Env Setup

#### 1- Create Environment
    $ python3 -m venv venv/

#### 2- Activating Environment
    # Linux / MacOS
    $ source venv/bin/activate
    
    # Windows (Command Prompt)
    $ venv\Scripts\activate

    # Windows (Git Bash)
    $ source venv/Scripts/activate

#### 3a- Creating and Installing Dependencies
    # Install pip-tools
    $ pip install pip-tools

    # Create requirements.in (already exist)
    $ touch requirements.in

    # Write dependencies in file
    $ echo "jupyterlab" > requirements.in
    
    # Compile into requirements.txt
    $ pip-compile requirements.in

    # Install dependencies
    $ pip install -r requirements.txt

#### 3b- Only Installing Dependencies
    $ pip install -r requirements.txt

#### 4- Starting Jupyter Lab
    # Linux / MacOS
    $ venv/bin/jupyter-lab --port=8888

    # Windows (Command Prompt)
    $ venv\Scripts\jupyter-lab

    # Windows (Git Bash)
    $ venv/Scripts/jupyter-lab
