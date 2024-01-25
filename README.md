# airflow
Airflow

## Installation
`python3 -m pip install -r requirements.txt`

This will get you compatible package versions.

## Initialise

`airflow db init`

## Create admin user

`airflow users create \`

`    --username admin \`

`    --firstname FIRST_NAME \`

`    --lastname LAST_NAME \`

`    --role Admin \`

`    --email admin@example.com`

REPLACE VARIABLES WITH PERSONAL INFOS.

## Configure

Edit the ~/Airflow/airflow.cfg file, to update the location of the dags folder to be absolute path to dags directory at this location.

Set up a user

`airflow users  create --role Admin --username admin --email admin --firstname admin --lastname admin --password admin`

## Launch

Do this after the config change to pick up the local dags location.

`airflow webserver --port 8080`

Then in a new terminal window

`airflow scheduler`

## Run (Hello World)



