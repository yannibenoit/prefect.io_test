# prefect.io_test
Testing https://www.prefect.io/

## Requirements
- Python 3.6+
- Docker and Docker-compose installed on the machine

## Install Prefect and dependencies
If you already have a virtual environment or you prefer to install prefect on
your base environement:
```bash
python3 -m pip install -r requirements.txt
```

### Install with Anaconda
If you use Anaconda or miniconda you can create a virtual environment
with the following commands:
```bash
conda env create -f prefect_env.yml
```
This will create a new environment, and not touch any of your existing environments, nor any existing Python installation.

Then activate the newly created env with:
````bash
conda activate prefect_env
```

To return to your root environment:
```bash
conda deactivate
```

## Start Prefect

Before running the server for the first time, run (configure Prefect for local orchestration)
```bash
prefect backend server
```

To start the server, UI, and all required infrastructure, run:
```bash
prefect server start
```

Once all components are running, you can view the UI by visiting http://localhost:8080

If you want to execute a flow from the server you'll need a prefect agent up
and running so let's start a prefect agent with the following command:
```bash
prefect agent start
```

More information [here](https://docs.prefect.io/core/getting_started/installation.html)
