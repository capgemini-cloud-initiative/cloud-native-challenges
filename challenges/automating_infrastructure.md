# Automating Infrastructure.



## The Challenge

Before you can start developing your cloud native application, there needs to be an environment available where you can deploy it to.
Normally you would have four environments for your applications:

1. Development
2. Test
3. Acceptance
4. Production



You can easily create these environments and their resources within the Azure portal, but that is not recommended. Manually creating these 
environments has several downsides:

- **Error prone**. Each time you are creating an environment there is a possibility for a typo.

- **Repetitive**. You need to do the same actions for each environment

- **Not maintainable**. It takes a lot of time if you need to update something in all the environments

  

In the last challenged you created a CI/CD pipeline for your web application. You automated the building, testing and deployment parts. 
Your mission in this challenge is to setup your infrastructure by code

# 

# No More Portal

Infrastructure as Code (IaC) is the management of your infrastructure using configuration files. IaC makes it easier to maintain them and 
prevents drift between the different environments. The configuration files would be stored in source control. This makes it possible to 
rollback to previous version if something goes wrong. If you need to change something within an environment, it can now also be reviewed using pull-requests.



There are several tools you can use for IaC on Azure. Azure provides native support for IaC via the Azure Resource Manager (ARM) templates. 
These templates can be a little difficult to understand for new developers. Microsoft has introduced a new language for developing ARM templates. 
The language is named [Bicep](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/bicep-overview	"Bicep Documentation").

# 

# Requirements

Choose your preferred tool for IaC and create the following Azure Resources:

- App Service plan
- App Service
- Key Vault



# Bonus point: Connecting It All Together

You have created a Key Vault, but an empty Key Vault is not very useful. The key vault usually stores sensitive information like a connection string. Create an Application Insights resource and store its instrumentation key in the Key Vault using IaC.



**Tip**: With Bicep, Blueprint and Terraform you have outputs. This returns the values from the deployment. You can use these values to create the secret.
