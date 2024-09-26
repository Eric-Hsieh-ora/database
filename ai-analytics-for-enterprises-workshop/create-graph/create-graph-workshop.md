# Setup User

## Introduction

You will be creating an Operational Property Graph inside of Graph Studio, one of the applications that's available in 23ai Autonomous Database. 

In this lab you will query the newly created graph (that is, `bank_graph`) using SQL/PGQ, a new extension in SQL:2023.
​

**_Estimated Lab Time: 20 minutes_**

### Objectives

In this lab, you will:
* Open up Graph Studio
* Create an Operational Property Graph
* Use SQL/PGQ to define and query a property graph

### Prerequisites

This lab assumes you have:
* Access to an Oracle Autonomous Database 23ai
- The bank\_accounts and bank\_transfers tables exist.

<!-- <if type="livelabs">
Watch the video below for a quick walk-through of the lab. The lab instructions on the left might not match the workshop you are currently in, but the steps in the terminal on the right remain the same.
[Change password](videohub:1_x4hgmc2i)
</if> -->

## Task 1: Download setup materials

1. Click [this link] (https://objectstorage.ap-singapore-1.oraclecloud.com/n/hutchhk/b/AIWorkshop/o/property-graph-workshop.zip) to download the zip file with our property graph setup materials.

2. Unzip the files. You should see these files available. Most of these files we will not be using throughout the lab, but are available if you would like to see what commands we chose to create the schema with (CreateKeys.sql) or the data that populates the tables that we've created (BANK\_ACCOUNTS.csv and BANK\_TRANSFERS.csv).

    ![Content of the zip file](images/1-unzip-workshop.png)

3. Back to the SQL action console.

    ![Back to console](images/im8-workshop.png)

3. Import bank account and transfer example data into your database.

    ![Load data](images/2-loaddata-workshop.png)
    ![Input two data](images/3-loaddata-workshop.png)
    ![Input two data](images/4-loaddata-workshop.png)
    ![Input two data](images/5-loaddata-workshop.png)
    ![Input two data](images/6-loaddata-workshop.png)
    ![Input two data](images/7-loaddata-workshop.png)
    ![Input two data](images/8-loaddata-workshop.png)
    ![Input two data](images/9-loaddata-workshop.png)
    ![Input two data](images/10-loaddata-workshop.png)

## Task 2: Create the Property Graph

1. Click graph studio.

    ![Navigating to graph studio](images/1-nav-graphs-workshop.png)

2. Sign into Graph Studio. 

    Username: ADMIN

    Password: Listed underneath Terraform Values -> User Password (AIWorkshop123#).

    ![Signing into Graph Studio](images/3-graph-studio-login-workshop.png)

3. Click on the Graph symbol on the left-hand side menu.

    ![Navigating to graph symbol on menu](images/4-nav-graphs.png)

4. Click </> Query.

    ![Graph homepage](images/5-query.png)

5. Use the following SQL statement to create a property graph called BANK\_GRAPH using the BANK\_ACCOUNTS table as the vertices and the BANK_TRANSFERS table as edges. Paste this into the text box:

    ```
    <copy>
    CREATE PROPERTY GRAPH BANK_GRAPH 
    VERTEX TABLES (
        BANK_ACCOUNTS
        KEY (ID)
        PROPERTIES (ID, Name, Balance, Email, Address, Zip, Phone_Number) 
    )
    EDGE TABLES (
        BANK_TRANSFERS 
        KEY (TXN_ID) 
        SOURCE KEY (src_acct_id) REFERENCES BANK_ACCOUNTS(ID)
        DESTINATION KEY (dst_acct_id) REFERENCES BANK_ACCOUNTS(ID)
        PROPERTIES (src_acct_id, dst_acct_id, amount)
    ) OPTIONS (PG_SQL);
    </copy>
    ```

    ![Query to create graph is inside textbox](images/6-create-graph.png)

6. Click Run. It should say Graph Successfully Created as a result at the bottom.

    ![Graph successfully created](images/7-graph-create-success.png)

## Task 3: Prepare the graph environment

1. Click the notebook icon on the left hand menu.

    ![Click notebook icon](images/8-nav-notebook.png)

2. Click DETACHED.

    ![Creating notebook button clicked](images/8-create-notebook-detached.png)

3. Click the start button.

    ![Notebook information being filled out](images/8-create-notebook-start.png)

4. You'll see a message saying that Graph Studio is being attached to an internal compute environment. The notebook will allow us to run PGQ queries against our bank schema, but first needs to spin up. It should take less than a minute.

    ![Graph Studio attaching to internal compute environment](images/10-attach-graph.png)

5. Once it completed, it should look like this. You can see the DETACHED message in the upper right corner turn to say ATTACHED with a green light.

    ![Environment was attached](images/11-notebook-success.png)

6. Load in memory the graph. Paste the following SQL statement into the text box:

    ![Load data in memory](images/1-load-in-memory.png)
    ![Load data in memory](images/2-load-in-memory.png)
    ![Load data in memory](images/3-load-in-memory.png)

7. You may now proceed to the next lab.

## Task 4 : Import the Notebook

1. Import Notebook
    ![Import Notebook](images/12-notebook-impart.png)
    ![Import Notebook](images/12-notebook1-impart.png)

2. Follow the notebook to complete this lab.

## Learn More

* [Introducing Oracle Database 23ai Free – Developer Release](https://blogs.oracle.com/database/post/oracle-database-23c-free)
