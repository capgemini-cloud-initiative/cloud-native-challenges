# Works on my cloud!

## The Challenge
Your mission is to create a new ASP.Net 5 MVC Application, running in Azure, which can be reached from the public internet.

# Requirements
- Deploy your first application in whichever way you want and verify you can reach it using your browser.

# A couple of options for you to try
- Publish right from Visual Studio 2019
- Use the Visual Studio Code Azure App Service Extension
- Azure DevOps Pipelines
- Github Actions
- Azure CLI
- Azure PowerShell

# Bonus points: Add a sprinkle of KeyVault to the mix
Suppose you have a secret or a connection string and you want to store it in a safe place. You don't want it in your source code repository. That would be bad. Azure allows you to store secrets, keys and certificates in a dedicated service, Key Vault, which integrates very nicely with ASP.NET.

- Deploy your MVC application AND an Azure KeyVault
- Store a secret in the KeyVault
- Have your application read the secret from the KeyVault and display it on the screen

Tip: Deploying a set of resources is very easy using Visual Studio 2019 Publish

We know...kinda defeats the purpose of KeyVault. But we're learning and we're not putting our credit card number in there...YET 🤫🐱:trollface:
