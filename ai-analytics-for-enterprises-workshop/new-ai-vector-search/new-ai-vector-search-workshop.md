# Exploring AI Vector Search

## Introduction

Welcome to the "Exploring AI Vector Search" workshop. In this workshop, you will learn what vectors are and how they are used in AI applications. We will cover the creation of vector tables, perform basic DDL operations, and dive into similarity search using some of the new SQL functions in Oracle Database 23ai. This lab is meant to be a small introduction to the new AI functionality that Oracle Database 23ai supports.

This lab will focus on AI Vector search at a very high level. If you're looking for an in depth workshop on AI Vector Search, check out the following labs:
* [Complete RAG Application using PL/SQL in Oracle Database 23ai](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3934&clear=RR,180&session=1859311324732)
* [7 Easy Steps to Building a RAG Application using LangChain](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3927&clear=RR,180&session=1859311324732)
* [Using Vector Embedding Models with Python](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3928&clear=RR,180&session=1859311324732)
* [Using Vector Embedding Models with Nodejs](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3926&clear=RR,180&session=1859311324732)

Estimated Lab Time: 20 minutes

### Objective:
In this lab, you will explore the new vector data type introduced in Oracle Database 23ai. You will create a vector table and perform basic DDL operations on the vectors. You will also learn about similarity search and how it relates to vectors, as well as use some of the new AI focused SQL functions in the database.

### Prerequisites:
- Access to Oracle Database 23ai environment.
- Basic understanding of SQL and PL/SQL.

## Task 1: Login the Data Science environment
1. Click [this link] (https://objectstorage.ap-singapore-1.oraclecloud.com/n/hutchhk/b/AIWorkshop/o/notebook-workshop.zip) to download the zip file with our notebook setup materials.

2. Unzip the files. You should see these files available. In the same time, copy the previous database setup section downloaded **Wallet_################.zip** file into the folder too. This file will be upload to the data science project later.

    ![Content of the zip file](images/1-unzip-notebook-workshop.png)

3. Navigate to Data Science.

    ![Navigate to Data Science](images/1-entry-data-science-workshop.png " ")

4. Into the Data Science Project.

    ![Navigate to Data Science Project](images/2-entry-project-workshop.png " ")

5. Into the Data Science Session.
    ![Navigate to Data Science Session](images/3-entry-session-workshop.png " ")

6. Into the Notebook Lab.
    ![Navigate to Data Science Notebook Lab](images/4-into-notebook-workshop.png " ")

7. Continue to sign-in.
    ![Navigate to Data Science Sign-in page](images/5-signin-workshop.png " ")

8. Sign-in success.
    ![Navigate to Data Science Sign-in page](images/6-welcome-workshop.png " ")

## Task 2. Import the Data science notebook

1. Into the Data Science Notebook Lab. You can extend the session first. Then upload this file that we downloaded and unzip.

    ![Extend session and upload file](images/6-extend-upload-workshop.png " ")

    Select the file and upload.
    ![Extend session and upload file](images/7-select-file-workshop.png " ")

    You can see the uploaded file in console.
    ![Extend session and upload file](images/8-upload-result-workshop.png " ")

2. Into the Terminal.
    ![Extend session and upload file](images/9-into-terminal-workshop.png " ")

3. In the Terminal, type in "sh go.sh" and press "Enter" to execute the shell file.
    ![Execute shell file go.sh](images/10-execute-shell-workshop.png " ")

4. Complete the configuration setup.
    ![Completed the go shell script](images/11-shell-complete-workshop.png " ")

5. Entry the notebook and start ot run the notebook.
    ![Start to execute the notebook script](images/12-start-notebook-workshop.png " ")

6. Let's start to run the notebook.

## Task 3: Integrate the JSON, Graph, and Vector AI

1. Let's start to run the notebook. You can press the **Shift+Enter** to execute the notebook script step by step.
    ![Execute the notebook script step by step](images/1-notebook-execute-workshop.png " ")
    Install require python libraries.
    ![Execute the notebook script step by step](images/2-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/3-notebook-execute-workshop.png " ")
    Connect to the database successfully.
    ![Execute the notebook script step by step](images/4-notebook-execute-workshop.png " ")
    Load Document.
    ![Execute the notebook script step by step](images/5-notebook-execute-workshop.png " ")

    ![Execute the notebook script step by step](images/6-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/7-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/8-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/9-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/10-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/11-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/12-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/13-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/14-notebook-execute-workshop.png " ")
    ![Execute the notebook script step by step](images/15-notebook-execute-workshop.png " ")

## Learn More

* [AI Vector Search User Guide](https://docs.oracle.com/en/database/oracle/oracle-database/23/vecse/oracle-ai-vector-search-users-guide.pdf)
* [23ai Release notes](https://docs.oracle.com/en/database/oracle/oracle-database/23/rnrdm/index.html)
* [7 Easy Steps to Building a RAG Application using LangChain](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3927&clear=RR,180&session=1859311324732)
* [Using Vector Embedding Models with Python](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3928&clear=RR,180&session=1859311324732)
* [Using Vector Embedding Models with Nodejs](https://livelabs.oracle.com/pls/apex/r/dbpm/livelabs/view-workshop?wid=3926&clear=RR,180&session=1859311324732)

## Acknowledgements
* **Author** - Killian Lynch, Database Product Management
* **Contributors** - Dom Giles, Distinguished Database Product Manager
* **Last Updated By/Date** - Killian Lynch, April 2024