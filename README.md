# datafactory
Learning, helping and teaching

This is a project to write a data pipeline that imports data from a public API and inserts it into the local databases that is scheduled to run every (5) minutes.
Nowadays, we are able to have information on flights around the world and track an aircraft in real time. For this we are going to use public API to extract data
using Airflow and save it:
* on MongoDB database for real time flights
* PostgreSQL for landed flights

## First step: retrieving data
  Here, we will have below scripts:
  * ingestion.py (import and transform data and load data )
  * model.py (contains tables of our database)
  * model-dag.py(The first DAG we will write is a DAG that will run our model script once, which will initiate tables in our database)
  * dag.py (script which will run our data ingestion script and export to db script daily
## Second step: Architecture
  
