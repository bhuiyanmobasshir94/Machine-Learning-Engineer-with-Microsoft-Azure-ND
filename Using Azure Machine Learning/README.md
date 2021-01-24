## Course Outline

Below is an outline showing the structure of the course, for your reference.

#### Lesson 1: Introduction to Azure Machine Learning

What You'll Build. We'll have a look at a preview of what you'll build on your final project.
Why Do ML in the Cloud? We'll go over some key reasons why you would want to do Machine Learning (ML) in the cloud. We'll look into some of the limitations of performing ML locally on your machine, as well as how the cloud addresses these limitations.
When to Do ML in the Cloud. Most of the time the cloud is your best option for ML. But we'll discuss a few edge cases in which using the cloud may not be the best route.
Customers of ML. We'll look at the different customers of machine learning, including both internal and external customers.

#### Lesson 2: Workspaces and AzureML Studio

The Azure ML Platform. We'll talk about the core features of the Microsoft Azure ML platform and how they enable you to be more productive as a data scientist or machine learning engineer.
Workspaces and Notebooks. Workspaces and notebooks are critical components of Microsoft Azure. We'll learn how these tools enable you to be a more effective data scientist—including the use of Jupyter to build and deploy machine learning models.
#### Lesson 3: Datastores and Datasets

Datastores and Datasets. Datastores and Datasets are a critical component of cloud computing. We'll learn how Azure allows you to easily integrate third party datasets and open datasets into our ML pipeline to quickly develop working solutions.

#### Lesson 4: Training models in Azure

Managing pipelines. We'll cover how to create a pipeline that you manage yourself using the console, which will alow you to make very small changes that can be run repeatedly.
Hyperparameters in experiments. We'll learn how to use hyperparameters in experiments, including how we can automate the creation of hyperparameters and make very small changes that create huge value in terms of prediction accuracy.

#### Lesson 5: Azure ML SDK

Creating pipelines. We'll talk about how the Azure ML SDK allows us to programmatically create pipelines. By automating the creation of pipelines, we can create more pipelines; also, our pipeline creation becomes a a repeatable process that other members of our team can follow.
Managing experiments. We'll learn how to use the SDK to manage experiments programmatically with Python, allowing us to easily rerun our processes using Python scripts.
Lesson 6: Automated Machine Learning and Hyperparameter Tuning
Automated ML and SDK. We'll discuss how we can use the Azure ML SDK to do Automated ML and create models more quickly and accurately.
Model Interpretation. We'll explore how model interpretation allows us to build solutions using Automated ML that we (and others) can more easily interpret, making visible the core features that are driving the model.

#### Project: Creating and Optimizing an ML Pipeline

In the project at the end of this course, you'll have the opportunity to create and optimize an ML pipeline. You'll do this both using HyperDrive and also Automated ML, so that you can compare the results of the two methods.


#### Additional Resources
1. [Microsoft Documentation: What is automated machine learning?](https://docs.microsoft.com/en-us/azure/machine-learning/concept-automated-ml)
2. [Azure Functions](https://azure.microsoft.com/en-us/services/functions/)
3. [What is elastic computing or cloud elasticity?](https://azure.microsoft.com/en-us/overview/what-is-elastic-computing/)
4. [Microsoft Documentation: Comparison between Azure data storage and on-premises storage](https://docs.microsoft.com/en-us/learn/modules/intro-to-data-in-azure/4-comparison-azure-and-on-prem-storage)
5. [**Tackling Bias in Machine Learning**](https://blog.insightdatascience.com/tackling-discrimination-in-machine-learning-5c95fde95e95)
6. [**A Survey on Bias and Fairness in Machine Learning**](https://arxiv.org/pdf/1908.09635.pdf)
7. [**How can your company perform a digital transformation?**](https://docs.microsoft.com/en-us/learn/modules/enable-digital-transformation/2-what-is-digital-transformation)
8. [Microsoft's official documentation on the Azure ML Plaftorm](https://docs.microsoft.com/en-us/azure/machine-learning/overview-what-is-azure-ml)
9. [Create an Azure Machine Learning Workspace](https://docs.microsoft.com/en-us/learn/modules/use-automated-machine-learning/create-workspace)
10. [Microsoft Documentation: Create Compute Resources](https://docs.microsoft.com/en-us/learn/modules/use-automated-machine-learning/create-compute)
11. [Explore Azure Machine Learning with Jupyter notebooks](https://docs.microsoft.com/en-us/azure/machine-learning/samples-notebooks)
12. [How to run Jupyter Notebooks in your workspace](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-run-jupyter-notebooks)
13. [the Microsoft documentation on describing data ingestion and processing](https://docs.microsoft.com/en-us/learn/modules/explore-concepts-of-data-analytics/2-describe-data-ingestion-process)
14. [Detect data drift (preview) on datasets](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-monitor-datasets)
15. [Azure Open Datasets](https://azure.microsoft.com/en-us/services/open-datasets/)
16. [Principle of Least Privilege](https://en.wikipedia.org/wiki/Principle_of_least_privilege)
17. [Article from Cybersecurity and Infrastructure Security Agency (CISA) (part of the US Department of Homeland Security)](https://www.us-cert.gov/bsi/articles/knowledge/principles/least-privilege)
18. [Pipelines](https://docs.microsoft.com/en-us/azure/machine-learning/concept-designer#pipeline)
19. [Datasets](https://docs.microsoft.com/en-us/azure/machine-learning/concept-designer#datasets)
20. [Compute resources](https://docs.microsoft.com/en-us/azure/machine-learning/concept-designer#compute)
21. [Registered models](https://docs.microsoft.com/en-us/azure/machine-learning/concept-azure-machine-learning-architecture#models)
22. [Published pipelines](https://docs.microsoft.com/en-us/azure/machine-learning/concept-designer#publish)
23. [Real-time endpoints](https://docs.microsoft.com/en-us/azure/machine-learning/concept-designer#deploy)
24. [What is Azure Machine Learning designer?](https://docs.microsoft.com/en-us/azure/machine-learning/concept-designer)
25. [Continuous Integration (CI)](https://en.wikipedia.org/wiki/Continuous_integration)
26. [Continuous Delivery (CD)](https://en.wikipedia.org/wiki/Continuous_delivery)
27. [data lineage](https://en.wikipedia.org/wiki/Data_lineage)
28. [What are Azure Machine Learning pipelines?](https://docs.microsoft.com/en-us/azure/machine-learning/concept-ml-pipelines)
29. [Microsoft documentation on tuning model hyperparameters](https://docs.microsoft.com/en-us/azure/machine-learning/studio-module-reference/tune-model-hyperparameters)
30. [Azure ML SDK documentation](https://docs.microsoft.com/en-us/python/api/overview/azure/ml/?view=azure-ml-py)
31. [Install the Azure Machine Learning SDK for Python](https://docs.microsoft.com/en-us/python/api/overview/azure/ml/install?view=azure-ml-py)
32. [the documentation for the dataset module](https://docs.microsoft.com/en-us/python/api/azureml-core/azureml.core.dataset)
33. [Players with salary wiki twitter - Social Power NBA Dataset](https://video.udacity-data.com/topher/2020/September/5f73bfb8_nba-2017-players-with-salary-wiki-twitter/nba-2017-players-with-salary-wiki-twitter.csv)
34. [Makefile](https://en.wikipedia.org/wiki/Makefile)
35. [An extensive documentation of all the things Experiments can do here](https://docs.microsoft.com/en-us/python/api/azureml-core/azureml.core.experiment.experiment?view=azure-ml-py)
36. [Pin all dependencies (& let pip sort ’em out)](https://www.promptworks.com/blog/pin-all-dependencies/)
37. [Tune hyperparameters for your model with Azure Machine Learning](https://docs.microsoft.com/en-us/azure/machine-learning/how-to-tune-hyperparameters)
38. [How Microsoft is applying AutoML to a variety of problems](https://www.microsoft.com/en-us/research/project/automl/)
39. [Video from Microsoft Research](https://www.youtube.com/watch?v=5ke9ZEvXJEk&feature=youtu.be)