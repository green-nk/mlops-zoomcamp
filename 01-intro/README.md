# Introduction to MLOps
In short, MLOps is the processes and set of best practices to put a ML model into production.


## MLOps Principle
![MLOps Principles](https://ml-ops.org/img/mlops-loop-en.jpg)

[MLOps principles](https://ml-ops.org/content/mlops-principles) consists of
* Design Phase: Identify ML use cases to satisfy the business requirements.
* Development Phase: Develop ML models with experiment tracking, a ML pipeline and model management to improve reproducibility and automate training and evaluation process.
* Operation Phase: Deliver ML models to be used by end users. Using deployment and monitoring to apply model observability.


### Why do we need MLOps
In summary, to properly serve ML models to end users and continuously operate on these services.

Components of MLOps
* Experiment Tracking: Log parameters, metrics and artifacts such as visualizations or prediciton results in order to compare among experiments and create a better model selection process.
* Model Registry: Keep track of model versions.
* ML Pipeline: Orchestrate a ML workflow by dividing scripts into multiple tasks and parameterizing inputs to improve reproducibility and automate ML development processes.
* Model Deployment: Put ML models to be used as a service.
* Model Monitoring: Apply model observability to ensure reliability of services and main model's performance.


### MLOps maturity levels
* Level 0 - No MLOps: No automation and all codes in the notebooks. Usually on development environment on POC phase.
* Level 1 - DevOps no MLOps: Automate releases such as unit and integration testing, CI/CD and keeping track of operational metrics but no experiment tracking or no reproducibility on ML models. Production environment on POC phase for simple projects.
* Level 2 - Automated Training: Experiment tracking, model management and ML pipeline are implemented but a little bit of model deployment practices no model deployment and monitoring. This level is suitable for 2-3+ ML use-cases.
* Level 3 - Automated Model Deployment: Automated model deployment with A/B testing and some model monitoring or some manual process is applied. This level is suitable for 5-6+ ML use-cases or 2-3+ important ones.
* Level 4 - Full MLOps Automated Operations: All processes are automated including model evalution is in ML pipeline. Model monitoring provides insights on how to improve the model. Usually apply for very mature and important use-cases.

In practice, not all the ML models need to be in the level 4 as the importance of each model is not the same. What you should do instead, you need to decide if a cost and time worth investing for a specific ML model.

The goal of this course is for students are able to apply ML maturity level on **level 2 at least** and for advanced students is to apply for around **level 3 to level 4**.


### MLOps tools and frameworks
* Experiment Tracking and Model Registry: MLflow or Weights & Biases
* ML Pipeline: Prefect or Apache Airflow or Kubeflow
* Model Deployment: Using Flask for web services.
* Model Monitoring: Using Prometheus, Evidently and Grafana for web services and using Prefect, MongoDB and Evidently for batch jobs.
* Best practices: Testing, Makefiles, GitHub Actions for CI/CD and IaC using Terraform.


## References
* [Getting started with MLOps](https://ml-ops.org/)
* [MLOps explained](https://www.youtube.com/watch?v=ZVWg18AXXuE&t=442s)
* [MLOps on MS Azure](https://github.com/microsoft/MLOps)
* [MLOps Maturity Model](https://learn.microsoft.com/en-us/azure/architecture/example-scenario/mlops/mlops-maturity-model)
* [Full Stack Deep Learning](https://fullstackdeeplearning.com/course/2022/)
* [Mde With ML](https://madewithml.com/)
* [CS 329S: Machine Learning Systems Design](https://stanford-cs329s.github.io/syllabus.html)
