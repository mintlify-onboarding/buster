# Datasource Onboarding

[Datasource Onboarding](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40.md)

[User Management](User%20Management%204cec064a73e14a619d3eaf694de7f698.md)

[Project Builder](Project%20Builder%207d59ea7b603648dfb0c80430255b2e2b.md)

[Embedding Documentation](Embedding%20Documentation%2050702aa0ad7e46cc8da8390e461e79fd.md)

# Getting Started

![Screen Shot 2023-10-25 at 12.03.59 PM.png](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Screen_Shot_2023-10-25_at_12.03.59_PM.png)

### What you will need

- **Read-only credentials** to your data source with access to schema and join information.
- Add our IP address to your Allowlist: `104.198.247.122`

### What will likely be helpful

- Any database/warehouse documentation your team has already prepared.
- An ERD diagram.

# Connecting to your data source

![Datasource Connection Page](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled.png)

Datasource Connection Page

### Creating the Read-Only User

Buster accesses your database/warehouse through a **read-only user.**  This user needs access to the following:

- All tables and columns that would be used in answering your users questions.
- Access to schema information such as schemas, tables, and columns.
- Access to all intermediate tables or columns that would be used to join across tables.

> *****Note: Enabling access to these tables and columns does not mean end-users will have access to query them. See Access Controls below to understand how Buster manages access to your tables and columns.*
> 

### Selecting Tenancy

In order to manage access to your data between customers, you will need to select your database architecture from one of the following options:

- **Single Tenant**
    
    This means that your customers’ data is broken out into different logical or physical locations.  If your SQL queries between customers look like the example below, this is likely what you should choose.
    
    ![Single tenancy diagram](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Single_Tenancy.png)
    
    Single tenancy diagram
    
    Single Tenant Example (Logical Separation):
    
    ```sql
    # Customer 1's query is using the customer_1 schema/database
    SELECT * FROM customer_1.users;
    
    # Customer 2's query is using the customer_2 schema/database
    SELECT * FROM customer_2.users;
    ```
    
- **Multi Tenant**
    
    This means that your customers share the same database and that records are separated on a row level, typically by some sort of customer identifier.  If your SQL queries between customers look like the example below, this is likely what you should choose.
    
    ![Multi tenancy diagram](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Multi_Tenancy.png)
    
    Multi tenancy diagram
    
    Multi Tenant Example:
    
    ```sql
    # Customer 1's query is using the WHERE clause to provision access.
    SELECT * FROM users WHERE users.id = 'customer_1';
    
    # Customer 1's query is using the WHERE clause to provision access.
    SELECT * FROM users WHERE users.id = 'customer_2';
    ```
    

### Select Environment

You’re able to select an environment for you datasources in Buster.  For any testing, development, or staging datasources, ****************************************************************************we recommend using the development environment****************************************************************************. This introduces an extra layer of security over data sources and prevents access to production environments during development.

### Data Source Types and Necessary Credentials

Depending on your data source, your credentials will look slightly different:

- **Postgres**
    
    **Host:**
    
    - This is where your database is active. *(Example: rds.amazonaws.com)*
    
    **Port:**
    
    - The port your database uses. *****(Example: 5432)*****
    
    **Database Name:**
    
    - The name of the database you are connecting to. **********************(Example: postgres)**********************
    
    **Username:**
    
    - The username of the read-only user you created. ********(Example: buster)********
    
    **Password:**
    
    - The password that you assigned to the read-only user at creation. **********************(Example: supersecure!)**********************
    
    **Schemas:**
    
    - The schema(s) you would like to connect to Buster.
    
    *********************************************************************************Note: If you’re customers are separated by schema, do not connect all schemas.  Only connect the schemas necessary to answer a ************SINGLE************ customers questions.*
    
    **SSH Config:**
    
    - If you require a connection through a bastion or jump host, please see: *[How to Connect to Buster via SSH](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40.md)*
- **********MySQL/MariaDB**********
    
    **Host:**
    
    - This is where your database is active. *(Example: rds.amazonaws.com)*
    
    **Port:**
    
    - The port your database uses. *****(Example: 3306)*****
    
    **Username:**
    
    - The username of the read-only user you created. ********(Example: buster)********
    
    **Password:**
    
    - The password that you assigned to the read-only user at creation. **********************(Example: supersecure!)**********************
    
    *********************************************************************************Note: If you’re customers are separated by schema, do not connect all schemas.  Only connect the schemas necessary to answer a ************SINGLE************ customers questions.*
    
    **Database Name(s):**
    
    - The name of the database(s) you are connecting to. **********************(Example: ecommerce_db)**********************
    
    *********************************************************************************Note: If you’re customers are separated by database, do not connect all databases.  Only connect the databases necessary to answer a ************SINGLE************ customers questions.*
    
    **SSH Config:**
    
    - If you require a connection through a bastion or jump host, please see: *[How to Connect to Buster via SSH](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40.md)*
- ********************SQL Server********************
    
    **Host:**
    
    - This is where your database is active. *(Example: rds.amazonaws.com)*
    
    **Port:**
    
    - The port your database uses. *****(Example: 3306)*****
    
    **Username:**
    
    - The username of the read-only user you created. ********(Example: buster)********
    
    **Password:**
    
    - The password that you assigned to the read-only user at creation. **********************(Example: supersecure!)**********************
    
    *********************************************************************************Note: If you’re customers are separated by schema, do not connect all schemas.  Only connect the schemas necessary to answer a ************SINGLE************ customers questions.*
    
    **Database Name(s):**
    
    - The name of the database(s) you are connecting to. **********************(Example: ecommerce_db)**********************
    
    *********************************************************************************Note: If you’re customers are separated by database, do not connect all databases.  Only connect the databases necessary to answer a ************SINGLE************ customers questions.*
    
    **SSH Config:**
    
    - If you require a connection through a bastion or jump host, please see: *[How to Connect to Buster via SSH](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40.md)*
- **BigQuery**
    
    **********************************Json Credentials:**********************************
    
    - This is the file that was given when you created the service account.
    
    ****Note: This user must have the**** `bigquery.jobs.create` ****role and have access to the schema information for the project you’re connecting.****
    
    ****************Project ID:****************
    
    - This is the identifier for the project you are connecting to. *********************(Example: buster_project)*********************
    
    ********************Dataset ID (Optional):********************
    
    - By default, Buster will pull in all datasets in a project. However, if you want to limit Buster to a specific dataset within a project, you would do that here.
    
    *********************************************************************************Note: If you’re customers are separated by dataset, do not connect all datasets.  Only connect the dataset necessary to answer a ************SINGLE************ customers questions.*
    
    ********************Restrict Tables (Optional):********************
    
    - By default, Buster will pull in all tables in a project.  However, if you want to limit Buster to specific tables within a project and dataset, you would do that here.
- **Databricks**
    
    **********Host:********** 
    
    - This is where your data warehouse is active. *(Example: cloud.databricks.com)*
    
    ****************API Key:****************
    
    - This is an API Key with read-only access to your cluster.
    
    **************************Warehouse ID:**************************
    
    - The identifier of the warehouse you are connecting to.
    
    ****************Catalog:****************
    
    - The name of the catalog that you are connecting to
- **Redshift**
    
    Reach out to us for Redshift connections: [founders@buster.so](mailto:founders@buster.so?subject=Question%20about%20Buster)
    
- **Snowflake**
    
    Reach out to us for Snowflake connections: [founders@buster.so](mailto:founders@buster.so?subject=Question%20about%20Buster)
    

### How to Connect to Buster via SSH

# Controlling Table and Column Access

![Tables and Columns Selection Page](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled%201.png)

Tables and Columns Selection Page

By default, Buster will pull in all tables and columns that are accessible through the read-only user you provisioned earlier.  However this does not mean that users are able to query those tables or columns.

****************************************************************************We recommend you turn off columns that:****************************************************************************

- Are deprecated
- Aren’t relevant to questions your users would ask
- Have data integrity issues

> *Note: You do not need to include tables or columns necessary for joins. Buster will still map across relationships in your database to answer questions.*
> 

### Access Control Validation

Buster validates every query that is generated with the access controls you specify during this step. In the screenshot above, we turned off the `email` and `phone` columns in the `contacts` table. Here is an example of a user dialog with these access controls:

<aside>
👤 **User asks: ‘**Show me all of our contacts’ emails.’

</aside>

<aside>
🤖 Buster begins query generation process…

Query generated is: `SELECT email FROM contacts;`

Buster validates if user has access to contacts table, then if user has access to email column.

In this case, Buster prevents query from running on database due to lack of user permissions.

******************Buster responds: ‘******************I’m sorry but I don’t have access to the data you are requesting.’

</aside>

You are able to change access at any time after onboarding.  **************************************************Be aware that if you turn off a table or column after it has been included in an answer to a user question, that user will no longer be able to retrieve data for that question.**************************************************

# Descriptions

We generate descriptions around your tables and columns that enables Buster to answer user questions more accurately.

While Buster can make assumptions about what tables and columns mean, we’ve found that Buster performs better when it has validated and correct context/documentation about your database/warehouse.  

A good way to think about this is to ask yourself the question: “If I was starting my job here today, would I know that `column_1` would mean `xyz`?”  

If the answer to the above is ‘no’, then you probably need to go in and change that description to align with your users’ questions.

By necessity we require all users onboarding their datasource to validate the following context:

- Table Descriptions
- Table Keywords
- Column Descriptions

You are able to change these descriptions at any time after onboarding.

### Table Descriptions and Keywords

![Table Descriptions Page](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled%202.png)

Table Descriptions Page

**********************Table Descriptions**********************

This description should be about **how** the table can be used to answer user questions. We recommend that you basically mention all the topics that can be answered using that table.  Here are some examples of good and bad descriptions for a table named `deals`.

- Good Example:
    - This table can be used to answer questions related to information about deals.  Information includes pricing info, start dates, end dates, status, company involved in the deal, etc.
- Bad Example:
    - This table can be used to answer questions about deals.

<aside>
🚨 We recommend keeping your descriptions below 3 sentences.

</aside>

****************************Table Keywords****************************

Your users may not refer to tables as they are named in your database.  For example you may have a table called `dim_orders` .  Relating to this table, your users will likely ask questions about orders, sales, transactions, etc.  Buster uses these keywords to more accurately answer user questions related to the table.

<aside>
🚨 We recommend having at least 5 keywords for each table.

</aside>

> *****Note: An individual keyword can actually be more than one word.*****
> 

### Column Descriptions

![Column Descriptions Page](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled%203.png)

Column Descriptions Page

Buster will attempt to generate descriptions about ******************what****************** your column is based on the column name, the context of the table as a whole, and 5 most recent samples values from the columns.  Typically, if your column name is human-readable (meaning it actually represents the data in the column) then Buster does a pretty good job of nailing these.

<aside>
🚨 **********************************************************************************************************************************We highly recommend you validate the description for each column.**********************************************************************************************************************************

</aside>

Here are a few recommendations for writing good column descriptions:

- Describe **what** the column is.
    - Good Example:
        
        `close_date` : this is the date assigned by a sales rep for when they expect the deal to be closed.
        
    - Bad Example:
        
        `close_date` : this is the close date
        
- Specify transformations that are necessary for a column.
    - Good Example:
        
        `price` : the buying price that the product was purchased at as a whole number.  Divide this number by 100 to get the currency amount.
        
    - Bad Example
        
        `price`: the price of the product
        
- If the column contains less than 10 values (enums, categories, etc.), we recommend passing those into the column description.  If the enums or values aren’t representative of what they actually mean, we recommend defining those.
    - Good Examples:
        
        `status`: the stage the deal is currently in. Stages are: [‘lost’, ‘won’, and ‘in progress’.]
        
        `status`: the stage the deal is currently in. Stages are: [1 = in progress, 2 = won, 3 = lost]
        
    - Bad Example:
        
        `status`: the stage of the deal
        
- If the column contains a JSON object, we recommend the keys and values within the description.
    - Good Example:
        
        `settings`: these are the settings associated with a user.  The JSON structure is as follows:
        
        ```json
        {
        	notifications: boolean, //representing if the user has notifications turned on
        	dark_mode: boolean, // representing if the user has dark mode turned on
        	profile_info: {
        		img_url: string // "string of the url that relates back to the user"
        	}
        }
        ```
        
    - Bad Example:
        
        `settings`: these are the setting associated with a user. it has notification, dark_mode, and profile info.
        

# Joins and Constraints

![Joins and Constraints Page](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Video_to_GIF.gif)

Joins and Constraints Page

Buster needs to understand how your tables and columns relate to each other in order to generate accurate and syntactically correct queries.  

If you are connecting a relational database, we pulled any foreign key relationships that you defined in your database.  However, there may be relationships that you haven’t explicitly defined in the database.  You would need to specify those here.

If you are connecting a warehouse, you will need to define all relationship for the tables you connected to Buster.

# Stored Values

![Stored Values](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled%204.png)

Stored Values

We have seen increased performance from Buster when we store and index distrinct string values.  These values are typically non-sensitive values such us product names, categories, event types, etc.  

A good example of this is if a user asks the question, “Show me our macbook m2 sales”.  But you have that product stored in your database as `m2_macbook`.  The query generated by Buster would likely be incorrect as the user asked for ‘macbook m2’.

Without storing these values, your users would have to know exactly how the value is stored in the database and reference it as such.  If you anticipate user questions around a column to specifically reference column values, then there is no need to store the values.

We’ve found that PII (Personally Identifiable Information) rarely needs to be stored.  Typically if a user question involves that information, it will be reference specifically, such as a birthday, address, email, or name.

> ******************************************************************************Depending on how many distinct values are stored in your database, this step will vary in completion time from a few minutes to a few hours.  You will still be able to ask questions of your data, but may be lacking the values needed for accurate queries.******************************************************************************
> 

# Fine Tuning

![Untitled](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled%205.png)

Buster is finally ready to start answering questions about your data!  We aren’t finished onboarding quite yet.  While documentation and context increase performance, we’ve found that there is “undocumented” context that Buster can learn from.

Here are a few examples of user questions that require some “undocumented context”:

- “Who are my top customers?”
    - What does that even mean? Top customer could be based on total revenue, total orders, average order size, etc.
- “Show me our ROI on ad spend from the last 3 months”
    - If ROI is not a column in your database,  a calculation of multiple columns is likely required.  How should that be done? Sometimes data can be messy.
- “Show me sales from the last 30 days”
    - What does a user expect when they see this? A report of each sale that occurred, a total sales number, or sales for each day from the last 30?

While Buster will attempt to make assumptions around questions, they may not always be correct.  This can be frustrating to end users.  Especially because they have zero context around your database and it may be difficult for them to guide Buster toward the right answer.

<aside>
📌 We recommend approving 25-100 question ↔ query pairs.  Each question that you approve is sent into our auto-training pipeline and Buster immediately starts learning from it.

</aside>

### Fine-tuning a Response

![Fine-tuning a question in Buster](Datasource%20Onboarding%206842921f039944f8a4cd5f618ccccf40/Untitled%206.png)

Fine-tuning a question in Buster

When you ask or view a question in this space, you will be able to see the question, the generated SQL, and the data returned by the query.

You are able to edit the question and the SQL directly.  You also have the capability to guide Buster toward the correct answer using the “Not quite right?” input box. In the case of the example above, I could ask Buster to break out the company sizes by 100 instead of 50.

Once you click approve, Buster immediately starts learning from the question and generated SQL code.  ******************************You can always come back and edit questions, SQL, or even remove an approval. Be aware that changing the training data will not change any generated SQL for users that have previously asked questions.******************************

# User Access Controls

Buster is able to provision access controls over your data through Row Level Policies (Multi Tenant) or Permission Groups (Single Tenant).  In either case, Buster implements security without the use of an LLM. 

Next →

[Project Builder](Project%20Builder%207d59ea7b603648dfb0c80430255b2e2b.md) 

On this page