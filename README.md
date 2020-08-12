# Terraform Servicenow Integration Update Set

This Integration/ App was installed from VCS and then exported into a single Update Set for testing on-Prem ServiceNow instances only.

Note:
-----------
**This is for testing purposes only!** <br />
**It is not the official HashiCorp app!** <br />
**Please do not use in production!** <br />


For the Officlal / Certified app please download from the:

**ServiceNow Store** - https://store.servicenow.com/

------------------

Upload:
-------------
1. Navigate to Update Sets -> Retrieved Update sets
1. Click "Import UpdateSet from XML" Select the xml file and upload

Commit:
--------------
1. Once upload completes click into the Terraform Update Set that is now listed
1. Once in the record - click on the button [Preview Update Set] 
1. This may result in errors depending on your version (I got 6 with Orlando) - in that case just select "Approve" / "Skip Remote Update" from teh far right of each error.
1. Once all Errors are skipped/ accepted hit the button that now appears - [Commit Update Set] 

This will install the terraform app.

#
