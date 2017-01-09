# Jedi_ChatBot

 **Prerequisite Resource:**
 
 Node.JS
 
 NPM
 
 Claudia.JS
 
 AWS IAM&LAMDBA
 
 AWS SDK for Node.js (Optional)

1. Create a AWS user grou with AWSLambaFullAccess+AdministratorAccess+AmazonAPIGatewayAdministrator
2. Conrigure Claudia.JS with AWS - (N.B. it is easiler to use aws sdk node command line to write the aws credentials to messgener folder)
e.g. creating/updating aws credentials
```
$ aws configure
AWS Access Key ID [None]: accesskey
AWS Secret Access Key [None]: secretkey
Default region name [None]: us-west-2
Default output format [None]:

$ aws configure
AWS Access Key ID [****]:
AWS Secret Access Key [****]:
Default region name [us-west-1]: us-west-2
Default output format [None]:
```

3. Build chat bot - adding the core javascript (here is bot.js)
4. Deploy ChatBot

```
$ claudia create --region us-east-1 --api-module bot

$ claudia update --configure-fb-bot
```
