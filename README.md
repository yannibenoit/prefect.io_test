# prefect.io_test
Testing https://www.prefect.io/

## Requirements
- Python 3.6+
- Docker and Docker-compose installed on the machine

## Install Prefect and dependencies

```bash
python3 -m pip install -r requirements.txt
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

More information [here](https://docs.prefect.io/core/getting_started/installation.html)