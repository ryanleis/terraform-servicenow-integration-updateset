# Terraform Servicenow Integration Update Set

This Integration/ App was installed from VCS and then exported into a single Update Set for testing on-Prem ServiceNow instances that cannot reach the ServiceNow Store.

Resources:
---------------
Follow the Steps in these resources:
Step By Step Guide - https://www.terraform.io/docs/cloud/integrations/service-now/index.html
Demo Walk- Thru video - https://www.hashicorp.com/resources/terraform-servicenow-new-integration-means-for-your-devops-workflows

Note:
-----------
This is for testing purposes only .... It is not the official HashiCorp app! <br />
**Do not use in production!** <br />

For the Official / Certified app please download from the: <br />
**ServiceNow Store** - https://store.servicenow.com/

Alternate method:<br /> https://store.servicenow.com/sn_appstore_store.do#!/store/help?article=KB0030267

------------------
# ServiceNow SetUp
Clone:
-------------
1. git clone https://github.com/ryanleis/terraform-servicenow-integration-updateset.git

Upload Update Set:
-------------
1. Navigate to Update Sets -> Retrieved Update sets
1. Click **"Import UpdateSet from XML"** Select the xml file and upload

Commit:
--------------
1. Once upload completes - click into the "Terraform" Update Set that is now listed
1. Once in the record - click on the button **[Preview Update Set]**
1. This may result in errors depending on your version (I got 6 with Orlando/Paris) - Just hit Close
1. In the case of errors - inspect the "Update Set Preview Problems" related list and select "Approve" or "Skip Remote Update" from the far right of each error.
1. Once all Errors are skipped/ accepted hit the button that now appears in teh top right corner - **[Commit Update Set]**

This will install the terraform app.


Add Terraform Service Catalog:
-------------------------------
1. Navigate to Service Catalog -> Catalog
1. Click the **"+"** in the top right coner to **"add content"**
1. Select **"Terraform Catalog"** and click **[Add here]**

This will install the Terraform Service Catalog which contains pre-built Catalog Items.

Connect ServiceNow to Terraform Cloud:
-------------------------------
1. Navigate to Terraform -> Config
1. Click "New"
1. Populate the following
    1. Set Org Name = Terraform Cloud Organization"
    1. Set Hostname = https://app.terraform.io
    1. Set API Team Token to the Terraform Cloud team API token
1. Click Submit




