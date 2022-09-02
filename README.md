# airflow-docker
 Basic tutorial on Apache airflow, which creates ML pipeline and compares model performances to select the best performing model.
 
 ## Running Airflow 2.0 with server Executor with Docker.
 
 ### System Requirements:                                                                                                                     
 - Install Docker
 - Install Docker-compose
 
**Step1:** Download docker compose file in airflwo-docker directory                                                                
Download docker-compose yaml file, Command : curl -LfO ‘https://airflow.apache.org/docs/apache-airflow/stable/docker-compose.yaml'            
**Step 2:** Create dags plugins and logs directory                                                                                       
**Step 3:** Exposing environment variables, command : echo -e “AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0”> .env                                 
**Step 4:** Initializing Airflow instance: docker-compose up airflow-init  (Creates admin user airflow)        

 --------------------------------                                                                        
Running all services present in docker-compose file, command : docker-compose up                                                       
Check status : docker ps (lists all containers)                                                                                  


### Airflow Instance                                                             
Open localhost:8080 in a browser        
user:airflow, pass:airflow   

<img src="https://user-images.githubusercontent.com/84242964/188059259-e7dce3b5-54cb-4357-a520-1d25990108ee.png" width="800" height="500">

