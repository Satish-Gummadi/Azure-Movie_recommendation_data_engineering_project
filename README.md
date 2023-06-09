# Azure-Movie_recommendation_data_engineering_project
Here I have created an End-to-End pipeline for movie recommendation on Microsoft Azure using its various services. I am attaching the Project report which explains everything about the project and project files along with it.

In this project we will be creating an End-to-End pipeline starting from loading the data from external source to sending the result to Gmail. We can summarize the entire project in following steps:
1) We will create a Microsoft Azure account to use the services. We will also create a resource group in order to group all the project files together.
2) We will create a Blob storage with hierarchical namespace enabled and create different folders for different purpose of storing files.
3) We will create Azure Databricks resource, mount it to our Storage using App registration and Key vaults. We will create a cluster in ADB and added our mounting code and movie recommendation code in different notebooks. We will run the codes by attaching the cluster to the notebooks and running them.
4) We will then create Azure Data Factory resource, create our pipelines using different activities such as Get MetaData, If Condition, Copy Data, Notebooks and Web Activity. We will also connect them, set their properties and published them.
5) We will create a Logic App resource and designe a workflow to receive data from pipeline and send result to our email. We will use URL generated by Logic Apps to connect our pipeline with Logic App. 
6) Later we will create a Storage event trigger and triggered the entire pipeline. 
7) We will check the entire pipeline run on Output section and in monitor, and we will check the movie recommendation email we receive on our Gmail at the end.

![Project Flowchart](https://github.com/Satish-Gummadi/Azure-Movie_recommendation_data_engineering_project/assets/111731023/19f4142c-c5c4-4299-8241-ddf4a2446e3c)

The whole process of creating the pipeline has been explained in the Project report attached. Please refer the same along with the project files attached.
