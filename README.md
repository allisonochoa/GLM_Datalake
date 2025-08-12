# Generalized Linear Model: Exploring Data Lake Architecture
![p.18g](/Assets/p.18g.png)
 
Tag along to discovering the lifecycle of building and deploying a Generalized Linear Model (GLM) Regression using Oracle Cloud tools and services.

Thanks to [Oracle MyLearn](https://www.oracle.com/mx/education/training/) for the incredible course: [Become a Big Data Administrator on OCI](https://mylearn.oracle.com/ou/learning-path/become-a-big-data-administrator-on-oci/82899). As this project is a direct result of my learning journey through it.

## 🔎 Background
For this project, I worked with sample data provided by **Oracle**. It showcases an IT company dedicated to selling both electronic and software products. 

### Dataset
The dataset provided consists of **7** tables:
- **channels**: sales channels (direct and indirect).
- **customers**: general customer info.
- **products**: product, product categories, cost, price, etc.
- **promotion**: promos types, costs, and dates.
- **sales**: products sold, date, quantity, sales channel, etc.
- **supplementary_demographics**: customer extended info.
- **times**: dates month, day, fiscal year, etc.

### Goal
Given the demographic, purchase, and affinity card data for a set of customers, predict numerical values using a multiple regression. I want to know the **number of years a customer remains at the same residence**. And, since this is a continuous variable, I will use the Generalized Linear Model algorithm.

###  Key Workflow Steps
1. [**Data Acquisition**](/1.%20Data_Acquisition/): downloaded CSV tables and documents provided by Oracle. 

2. [**Data Lake Architecture**](/2.%20Datalake_Architecture/): uploaded CSV dataset to Oracle Object Storage. Created an Autonomous Database and provisioned it.

3. [**Connections**](/3.%20Connections/): connected ADB to code editor, created users, generated a token to save my credentials, and created *channels* and *promotions* external tables.

4. [**Machine Learning**](/4.%20Machine_Learning/): OML user creation and GLM regression model building.

5. [**Data Catalog**](/5.%20Data_Catalog/): Virtual Cloud Network and Data Catalog creation in OCI. Dynamic Group and Dynamic Group Policy creation for Data Asset. Object storage and Data Asset connection. Data Asset harvesting.

6. [**Data Flow**](/6.%20Data%20Flow/): Dynamic Group and Dynamic Group Policy creation for Data Flow. Spark Application run.

## 🛠️ Built With
- **Oracle Cloud**: the project's environment. Including Oracle Autonomous Database, Oracle Machine Learning Notebooks, Oracle Object Storage, Oracle Data Catalog, and Oracle Data Flow with Spark.

- **SQL and PL/SQL**: languages. The backbone of the architecture and model.

- **Visual Studio Code**: editor for database management and SQL queries execution.

- **ChatGPT & Gemini**: AI assistants. Used for troubleshooting and further clarifications.

## 📋 Prerequisites
- **OCI**: You'll need an Oracle Cloud account. For must of the project, an [Oracle Cloud Free Tier](https://www.oracle.com/mx/cloud/free/) account will work just fine.
- **SQL**: A basic knowledge of SQL is advised in order to understand the queries provided.
- **Code Editor**: You'll need to install a code editor like VS Code or Oracle SQL Developer. I worked with **VS Code**.

## 🧠 Key Learnings
-  **End-to-End ML Lifecycle in Oracle Cloud**: I gained hands-on experience implementing a full machine learning pipeline within the *Oracle Cloud Infrastructure* (**OCI**) ecosystem. 

- **Oracle Autonomous Database & OML**: I worked directly with the *DBMS_DATA_MINING* package to build a *GLM* regression model, enabling advanced tasks such as:
    * Setting algorithm parameters
    * Enabling automatic data preparation
    * Accessing prediction details and feature influence

- **Access & Security Configuration in OCI**: I was able to understand how *Resource Principals*, *Dynamic Groups*, and *IAM Policies* work together to enable secure service-to-service communication.

- **Debugging in Oracle Cloud**: I also became familiar with interpreting and resolving cloud-specific errors like:
    * DCAT-20127 *Data Catalog* access issue
    * Service limit exceeded errors in *Data Flow*
    * Invalid *IAM Policy* and *Dynamic Group* configurations

- **Best Practices in Data-Driven Projects**: finally, I learned to manage data access, model artifacts, and documentation for reusability and reproducibility of ML workflows.

## 📝 Conclusions
This project provided me with valuable hands-on experience in the world of *Big Data* and a practical understanding of data lake architecture. Throughout the process, I discovered the power and flexibility of the *Oracle Cloud Infrastructure* (**OCI**) and its suite of integrated services. As well as experienced how smoothly **OCI** connects with external tools like *Visual Studio Code*, enhancing the development workflow.

Most importantly, this journey allowed me to successfully build and deploy a *Machine Learning* regression model, applying real data to generate predictions. A rewarding step into the application of AI in real-world scenarios throughout my *Data Analysis* journey.

# Acknowledgments
The information presented is based on the learning materials and lab exercises provided by *Oracle* as part of the [Oracle MyLearn](https://www.oracle.com/mx/education/training/) course on how to  [Become a Big Data Administrator on OCI](https://mylearn.oracle.com/ou/learning-path/become-a-big-data-administrator-on-oci/82899). All the data files, model templates, and step-by-step instructions were originally created and distributed by *Oracle*.

My intent is to document my personal learning journey while following this hands-on lab, share useful insights I gained, and demonstrate how I applied the knowledge using *Oracle Cloud Infrastructure* (**OCI**) tools such as:

- *Oracle Autonomous Database*
- *Oracle Machine Learning (**OML**)*
- *Oracle Object Storage*
- *Oracle Data Catalog*
- *Oracle Data Flow*

Full credit for the original educational content goes to *Oracle*.