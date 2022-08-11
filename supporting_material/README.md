# Note
While running the AWS commands using either create.sh or update.sh file, if you face permission denied error, then you will have to grant the execute permission to the owner (yourself) explicitly as:
```
chmod +x update.sh 
chmod +x create.sh
``` 

# Running CloudFormation test script for section 1 (Getting Started)
`scripts/create.sh testStack cloudFormationScriptTest.yml`  
`$1` is stack name  
`$2` is the template body file

# Running CloudFormation test script for section 3 (Network Infrastructure) Create Internet Gateway
`scripts/create.sh ourInfraDemo network_infra/ourInfra.yml network_infra/ourInfra.json`  
`$1` is stack name  
`$2` is the template body file
`$3` is the param json

# Running CloudFormation test script for section 3 (Network Infrastructure)  Attach VPC and Internet Gateway
`scripts/update.sh ourInfraDemo network_infra/ourInfra.yml network_infra/ourInfra.json`  