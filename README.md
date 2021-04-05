# Data Science Study Dataiku_LeaseCosts  

Data analysis of Auto Dealerships Lease Opportunities for 2021-2025.  
Objetive: Create a dashboard proposal based on the observations, measures, metrics and KPIs. Based on 48 variables over a period of 15 years.  
Method: CRIPS-DM (Cross-Industry Standard Process for Data Mining).    
Tools: Interview / BPM light, Data dictionare/concept, Google Drive, Excel, Postgres, GCP, Data Science Studio Dataku, Odoo and Github. On DEV (BigQuery - Tableau - Celonis)       
       
# Overview of the result:  
**Dashboard:**
![image](https://user-images.githubusercontent.com/72107370/113620921-f51b5700-9628-11eb-8d90-51256ad596d6.png)  

**Report:**   
 ![image](https://user-images.githubusercontent.com/72107370/113622356-de75ff80-962a-11eb-8715-e484b732bb75.png)  
  
    
# Method:
**CRIPS-DM (Cross-Industry Standard Process for Data Mining).**  
![image](https://user-images.githubusercontent.com/72107370/113621583-c782dd80-9629-11eb-888d-94f986d1bbca.png)  
 - **Business understanding** – What does the business need?  
 - **Data understanding** – What data do we have / need? Is it clean?  
 - **Data preparation** – How do we organize the data for modeling?  
 - **Modeling** – What modeling techniques should we apply?  
 - **Evaluation** – Which model best meets the business objectives?  
 - **Deployment** – How do stakeholders access the results?  
Reference: https://www.datascience-pm.com/crisp-dm-2/ 
  
    
# Data understanding  
**Input:** Functional requirements of the client, sources of information (GoogleDrive, Excel).  
**Output:** Data engineering/architecture phase, connection of data sources and creation of the work environment with Dataiku.   
(Configuration of Dataiku, plugins and APIs of Google Cloud Platform)  

Documentation:  
- https://www.dataiku.com/product/get-started/linux/   
- https://launchpad-dku.app.dataiku.io/   
- https://www.dataiku.com/product/plugins/googledrive/  
- https://www.dataiku.com/product/plugins/googlesheets/  
- https://cloud.google.com/sdk/gcloud/reference/iam/service-accounts/keys/create  
- https://drive.google.com/drive/folders/1ld89u6kbTpWj0Z_2Jjio5mWLb_j81Q2o?usp=sharing  

**View of Google Drive conector in Dataiku:**  
![image](https://user-images.githubusercontent.com/72107370/113625561-10896080-962f-11eb-8000-98640ffc4fc8.png)   
     
# Data preparation  
**Input:** Data engineering/architecture phase, connection of data sources and creation of the work environment with Dataiku.    
**Output:** Flow base on Dataiku with a first dataset on BD(postgres) prepared for analisys.  
(Dataiku, plugins Anonymization and Postgres)  

The Dataiku visual flow allows coders and non-coders alike to easily build data pipelines with datasets, recipes to join and transform datasets, and the ability to build predictive models. Dataiku includes over 90 built-in data transformers for common data manipulations like binning, concatenation, currency conversions, date conversions, filtering, splitting, and more.  
  
The main steps taken for data processing were:  
- **Data labeling** (categorical and numerical data).  
- **Data cleaning** (incontinences, empty and duplicated data).  
- **Data transformation** (Date and geospatial information).  
- DEV **(Data Anonymization, Balancing, and Shuffling)** It is not part of the scope of the project but some actions were taken.  

**View of recipe Prepare of Dataiku:**  
![image](https://user-images.githubusercontent.com/72107370/113628594-197c3100-9633-11eb-8b45-049b1b2d6689.png)  
  
  
The visual flow also has code and reusable plugin elements for customization and advanced functions (eg anonymation).  
- https://www.dataiku.com/product/plugins/anonymizer/  
  
Dataiku provides built-in geospatial transformation functions when working with geospatial data.  
- https://doc.dataiku.com/dss/latest/preparation/geographic.html  
- https://www.dataiku.com/product/plugins/geocoder/  


**View of general flow in Dataiku:**  
  ![image](https://user-images.githubusercontent.com/72107370/113629910-0ec29b80-9635-11eb-968b-cda5f0de4a54.png)  
    
    
# Modeling
**Input:** Flow base on Dataiku with a first dataset on BD(postgres) prepared for analisys.    
**Output:** Exploratory Data Analysis, Charts and Graphs, Geospatial Analytics, Statistical Analysis, Dashboards and Integrations with Tableau.  
(Dataiku, plugins for export to Tableau)  
