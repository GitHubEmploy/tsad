# Anomaly Detection Framework

_________________

[![PyPI version](https://badge.fury.io/py/anomaly-detection-framework.svg)](https://pypi.org/project/anomaly-detection-framework)
[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.org/project/anomaly-detection-framework)
_________________

Anomaly-Detection-Framework is a platform for Time Series Anomaly Detection Proplems. Give the data to platform get the Anomaly Labels with scheduled time perioeds. That is simple is that!!!
Anomaly-Detection-Framework unables to Data Science communities easy to detect abnormal values on a Time Series Data Set. It is a platform which can run on Docker containers as services or python by using its modules. It also has the web interface which allows us to train - prediction - parameter tuning jobs easly.

##### Key Features
-   **Web Interface**: 

    It is web interface which allows us to connect data source and execute Machine Learning processes. You may create tasks according to your data set. These tasks are train models, Anomaly Detection Prediction, Parameter Tunning For Train Models.
    - *Menu*
        - [Data Source Configuraitons](http://127.0.0.1:7002/configs)
        - [Crate Task](http://127.0.0.1:7002/configs)
        - [Job Center](http://127.0.0.1:7002/ml_execute)
        - [Dashboard](http//:127.0.0.1:7002/dashboard)
    
-   **Schedule Machine Learning Jobs**:

    Three main process are able to initialized from platform Train, prediction and Parameter Tuning. Each Process can be scheduled Daily, Monthly, Weekly Hourly, etc with given time. In addition to that, you may run your Machine Learning processes real time.
    
-   **Dashboard Visualization**:

    When your data have connec to a data source and assign Date Indicator, Model Dimensions (optional), and feature column from Create Task  Menu [Create Task](http//:127.0.0.1:7002/query?messages=True), you may see the dashboard from [Dashboard](http//:127.0.0.1:7002/dashboard) Menu.
    
-   **Data Sources**: 
    Here are the data source you can conect with your SQL queries:
    
    - Ms SQL Server
    - PostgreSQL
    - AWS RedShift
    - Google BigQuery
    - .csv
    - .json
    - pickle
    
- **Models**:

    There are 2 Anomaly Detection Algorithm and FBProphet Anomaly Detection Solution are running on the platform.
    - LSTM
    - FBProphet
    - Isolation Forest
    
- **API Services**:

    There are 4 Services run on the platform.
    - Machine Learning Schedule Services
    - LSTM Model Service
    - FbProphet Model Service
    - Isolation Foreset model Service
    

- **Docker Compose Integration**:

    Threse 4 containers are running on containers as services.
    - ml_executor-services
    - model-services-iso_f
    - model-services-lstm
    - model-services-prophet

---
    
# Running Platform
#### Local
// Blue. Like all Byzantine agreement protocols, SCP makes no assumptions about the rational behavior of attackers.

** 1. You Have to Specify you directory **

```
import anomaly_detection as ad_exec

ad = ad_exec.AnomalyDetection(path='./Desktop', environment='local)
ad.init(apis=None)

```

** 1. You Have to Specify you directory **

#### Docker-Compose

<div class="text-purple">
  This text is purple, <a href="#" class="text-inherit">including the link</a>
</div>

Connection PostgreSQL

![connection_postgre](https://user-images.githubusercontent.com/26736844/83358571-27ab5200-a37d-11ea-95b9-b91b1ee38269.gif)


Create Tasks 

![create_tasks](https://user-images.githubusercontent.com/26736844/83358834-e320b600-a37e-11ea-91d7-a0dbb351ea91.gif)


