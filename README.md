# Sprints-Graduation-project

This repo represents the final graduation project (covid dataset ) for Sprints data engineer masterclass .


thanks to : Eng. Ahmed Reda and Eng. Amr Saleh 



# Main Business Requirement

this project aims to Create an automated pipeline workflow from ingestion till visualization for COVID dataset

# Requirements

show on a map the top 10 ranking countries in death rate

show on a map the top 10 ranking countries in testing rate

show the top 10 ranking countries in testing rate on a pie chart

# Technical Requirements

Create Folder on the cloudera Virtual Machine

Upload dataset “covid-19.csv” into VM using WinSCP

Load the dataset to HDFS directory using HDFS cli commands in a shell script

Create database on Hive and create schema for each Hive loading stage

I. 1st Hive staging table for pointing to dataset location to select data from

II. 2nd Hive ORC table is partitioned by Country and data are loaded dynamically into it to speed query

III. 3rd Final hive table to generate the final report which will generate output file to be visualized

Create an Oozie workflow actions from to run the HDFS shell script and execute the Hive queries

Create power bi dashboard to show the results
