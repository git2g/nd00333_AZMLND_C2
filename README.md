# Udacity Nanodegree Project 2 - Operationalizing Machine Learning

Using Azure Machine Learning, this project configures a cloud-based machine learning production model, deploys it, and consumes it. In addition, this project also creates, publishes, and consumes a pipeline

## Architectural Diagram
![](images/a.png)

## Key Steps
1. Authentication - Installed az ml, created service principal and shared the wksp with sp (not using the lab's, instead, have a subscription from work that I'm using):
![](images/1.png)
![](images/2.png)

2. AutoMl - created AutoML exp and ran the classification based exp in a NC compute cluster:
![](images/3.png)
![](images/4.png)
![](images/4a.png)
![](images/4b.png)
![](images/4c.png)
![](images/5.png)
![](images/5a.png)
![](images/5b.png)
![](images/5c.png)
3. Deployed the model using ACI and enabled authentication
4. Enabled application insights using `logs.py` 
![](images/6.png)
![](images/7.png)
5. Load the swagger.json of model using the provided swagger client script:
![](images/8.png)
6. Executed `endpoint.py` to consume the model endpoint with test data and benchmarked:
![](images/9.png)
![](images/10.png)
7. Created and published the pipeline using the Jupyter Notebook from starter files:
![](images/11.png)
![](images/12.png)
![](images/12a.png)
![](images/13.png)
![](images/14.png)
![](images/14a.png)
![](images/15.png)
![](images/15a.png)
## Screen Recording
[https://www.screencast.com/t/mbY4yZN7f8M7](https://www.screencast.com/t/mbY4yZN7f8M7)

## Standout Suggestions
In the future, we could have the flexibility to load the swagger.json in Postman or other swagger clients rather than run the provided script as it had it's own challenges, which is unecessary to highlight the point of this task - operationalizing a ml pipeline. 
