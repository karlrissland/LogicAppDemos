# LogicApp DevOps Demo
I get this question all the time... how do you incorporate a LogicApp into your Ci/Cd process?  While it isn't that difficult, it can be a little complex since a LogicApp actually lives within an ARM template.  So have end up with a template within a template.

## Overview
### What the demo does
Keeping it really simple.  The LogicApp will trigger when a new file lands on a storage account.  All the Azure Services and the LogicApp code is deployed with a pipeline (GitHub/ADO).  Once deployed, everything is running, no need to manually authorize the LogicApp Connection.

### Technologies Used
* Azure Storage
* Azure KeyVault
* Azure EventGrid
* Azure LogicApps
* Azure Resource Manager Templates
* Github Actions
* Azure DevOps pipelines