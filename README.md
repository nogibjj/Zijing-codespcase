# Data Script with Databricks
This is Zijing's project 1 repo, which contains a big data script that use Databricks API and Streamlit app to show word cloud for job salary analysis. 

Demo link: 
Dataset: https://www.kaggle.com/code/raghurayirath/plotly-data-science-job-salary-dataset-eda/data

## Project Structure


## Test CLI
databricks clusters list --output JSON | jq
databricks fs ls dbfs:/
databricks jobs list --output JSON | jq

## CLI Query 
  query-job-avg-salary  Find job average salary
  query-most-n    --n      Find N most pay job, default=5

chmod +x query.py
./query.py query-most-n --n 5 
./query.py query-job-avg-salary

## Microservice
streamlit run app.py --server.enableCORS=false