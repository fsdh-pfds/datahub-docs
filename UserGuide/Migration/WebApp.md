# Migrating or Offobarding Your Web Apps

This document provides instructions about:

*	migrating your web apps from the proof-of-concept (POC) environment to your new FSDH workspace in the production (PROD) environment
*	offboarding your web apps from the POC environment should you not be shifting your research to the PROD environment

__Please note: The FSDH team will establish a cutoff date for active analysis and experimentation in the POC environment as well as a final date by which all databases, storage, web apps, and Databricks resources must be migrated or offboarded. Once finalized, these dates will be communicated in this documentation, by general email and via in-platform announcements to ensure all workspace leads are aware of all important deadlines in order to avoid unintended data loss.__

## A. Migrating from POC to PROD

In order to migrate your web apps, you must have a new workspace in the PROD environment. The FSDH team will provide more information when it becomes available and will provide support as requested. 

To migrate your web apps from the POC environment to the PROD environment, you can simply redeploy your web app in PROD using your existing `docker-compose.yml` file stored in your Git repository. Please stop your web app in the POC environment once you have successfully deployed it in the PROD environment.

**NOTE:** You may need to update your images or `docker-compose.yml` file, especially if you use any configurations specific to the POC environment, such as PostgreSQL connection strings or Databricks connection strings.

## B. Offboarding from POC

To offboard your web apps from the POC environment, you can simply stop your web app in the FSDH portal. The app can then be redeployed on a different platform or environment using your images.

## C. Support

If you encounter any issues during the migration process, please contact the Federal Science DataHub support team by submitting a Support Request. Our team is happy to assist with migration or offboarding your web app.
