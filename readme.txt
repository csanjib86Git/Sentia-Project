The attached script will ask for the SubscriptionId, the name of the template.json and rule.json files
a login is required after that 
after login the script execute the below steps
it will reate a group with the name "GRP-SentiaWE7" in location "West Europe".
A storage account with the name "sentiaazurestorage123" in the created group.
A Virtual Network in the above created Resource Group with three subnets, using 172.16.0.0/12 as the address prefix
Apply the following tags to the resource group: Environment='Test', Company='Sentia'
Create a policy definition with the name "allowed-resourcetypes" using a template and parameter file, to restrict the resourcetypes to only allow: compute, network and storage resourcetypes
It will create an assignment with the name "allowed-resourcetypesassignment" and Assign the policy definition to the subscription and resource group created previously