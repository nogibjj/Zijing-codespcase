# Data Script with Databricks
This is project 1.

Demo link: 
Dataset: 

#Test CLI
databricks clusters list --output JSON | jq
databricks fs ls dbfs:/
databricks jobs list --output JSON | jq

#CLI Query 
  query-job-avg-salary  Find job average salary
  query-most-n    --n      Find N most pay job, default=5

chmod +x query.py
./query.py query-most-n --n 5 
./query.py query-job-avg-salary

#Microservice
streamlit run app.py --server.enableCORS=false