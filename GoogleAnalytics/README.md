# Site analytics Notebook
## Notebook uses Google analytics api for statistical data calculations.
## Important notes:
* Need to create Google Service account and put p12 security key (rename it to service-key.p12) into **RESOURCES_FILE_PATH** folder
* Need to create Google Analytics View and change **ANALYTICS_VIEW_ID** to the specific View ID
* Need to provide Google Service account email (**SERVICE_ACCOUNT_EMAIL** variable)
* Need to add Service account email to allowed users in Permission section of the specified Analytics View