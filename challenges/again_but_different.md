
# Do it again, but different.

## The Challenge
In the last challenge you created a web application and deployed it to Azure. It didn't matter how you deployed, just that it could be reached from the public internet. In a real-world scenario you wouldn't do these actions by hand, but it would be automated by a pipeline,

Your mission in this challenge is to setup a Azure DevOps pipeline that will build, test and deploy your web application. 

# I :heart: YAML
In Azure DevOps you can create a pipeline using the GUI (Classic UI), but there are signs that it will be deprecated soon. Microsoft also recommends you start using YAML instead. This has some great advantages compared to the Classic UI:
 - Encourages collaboration
 - Versioning

# Requirements
- Setup a pipeline that will only be triggered when a new commit is made to the master/main branch
- The pipeline should do the following actions:
	* Build project.
	* Run unit tests.
	* Publish project.
	* Deploy to Azure.

# Bonus point: Code Coverage
Having unit tests ensures that your code meets a certain quality standard. A good test coverage also helps when you want to refactor your code. 
In Azure Pipelines you can view the coverage of your unit tests. The coverage results can be used to find code paths that aren't currently covered by your tests.

- Add unit tests to the web application
- Run the unit tests in the pipeline
- Analyze and publish coverage results

Tip: You can use JaCoCo or Cobertura to create the test coverage results

Having to click on a build definition to view your test coverage isn't an ideal workflow. There is an Azure DevOps [extension](https://marketplace.visualstudio.com/items?itemName=shanebdavis.code-coverage-dashboard-widgets) you can install to have a widget that fixes this issue. The widget can be added on your custom dashboard to have an easy access to the test coverage.

