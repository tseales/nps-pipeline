# National Park Services (NPS) API Exploration
*[NPS API](https://www.nps.gov/subjects/developer/index.htm) Data Pipeline Creation - Python, AWS/Snowflake, dbt*
## Goal
Utilize the National Park Services' (NPS) API for purposes of:
  - Practicing data pipe-lining
  - Locally creating datasets derived from API calling
  - Inserting Pandas DataFrames in cloud-based databases *(with original intent of AWS specifically)*
  - Updating AWS database from local Python functions

The code contained in the Jupyter Notebook mainly concerns migrating local datasets to an AWS or Snowflake cloud database. The first path of red in the diagram below, indicates an original intent to ultimately house the data in AWS Redshift for further use with dbt. The second path of red emerged due to costs of resources for AWS Redshift, with no trial period available. Although migrating the data held in the created S3 bucket to Snowflake was successful, a notable number of NaNs were present in the destination tables. No root cause could be identified for this, thus creating the green path of migrating the locally-hosted tables directly to Snowflake - for further use with dbt and Tableau. \
*After dbt was successfully connected to the Snowflake warehouse, the end of trial-periods encumbered the final intention of displaying findings in Tableau.*


![NPS-Diagram](https://github.com/user-attachments/assets/2eb7e3a2-a601-4337-8801-b4e11fbce117)
