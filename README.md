# bike-company-spark

This project will be an an addendum to the [bike-company-hadoop](https://github.com/leorickli/bike-company-hadoop/blob/main/README.md#bike-company-hadoop) project. This time, I will use Spark for data analysis, most specificaly, PySpark to analyse the SQL queries made on the last project and Spark ML to make a linear regression model for predicting the total sales of the top 10 products in this dataset.

*Apache Spark is an open-source, distributed computing system that is designed for big data processing and analytics. It was developed at the AMPLab at the University of California, Berkeley and later donated to the Apache Software Foundation, where it became an Apache project. Spark is built to be fast, flexible, and easy to use, making it one of the most popular frameworks for big data processing.*

The following Hadoop tools and others were used:

**Google Cloud Platform (GCP)**: The cloud chosen for this project. I chose this cloud because of Dataproc, this way I don't have to worry about the admin overhead that deploying an on-premises Hadoop infrastructure would give me.
**PySpark**: This will be used to translate the SQL queries used on the bike-company-hadoop](https://github.com/leorickli/bike-company-hadoop/blob/main/README.md#bike-company-hadoop) project to Spark, using Python in the process. Two more examples are added to show the features of this tool.
**Spark ML**: A linear regression model will be used for predicting the total sales of the top 10 products in this dataset. Using Python, Spark ML is the Spark tool for this job.

I will be using the same dataset on [this repository](https://github.com/leorickli/rox-test), specifically in [this "cleaned_files" folder](https://github.com/leorickli/rox-test/tree/main/cleaned_files). Feel free to check it out if you want to see the cleaning and EDA procedures in the ["cleaning_eda_notebooks"](https://github.com/leorickli/rox-test/tree/main/cleaning_eda_notebooks) that were made in the dataset. 

## Deploying the infrastructure

I created simple Dataproc cluster (1 master, 1 worker) to deal with the most demanding machine learning job. This dataset is very small so I had no trouble in processing power.

There is a [Jupyter notebook](https://github.com/leorickli/bike-company-spark/blob/main/spark_notebook.ipynb) that you can find in this project, it contains the data analysis and machine learning for the project.

## Conclusions

Machine learning is all about experimentation, there is a big margin for experimentation and feature engineering in this dataset. The model works, but its still very unrefined, it has a lot of potential for future exploration.
