Summary

Every company has the same goal: to deliver value to customers and maintain customer satisfaction. To achieve this, an organization needs to be fast in integrating customer feedback and release new features.

It is possible to manually deploy every release for a small product. However, this is not viable for a product that has thousands of microservices developed by hundreds of engineers. A delivery pipeline is essential for continuous and automated deployment of new functionalities.

A delivery pipeline includes stages that can test, validate, package, and push new features to a production environment. It is common practice for the main branch commits to proceed through all stages of the pipeline to reach the end-users. Overall, a delivery pipeline is triggered when a new commit is available. The new changes should traverse the following stages:

Build - compile the application source code and its dependencies. If this stage fails the developer should address it immediately as there might be missing dependencies or errors in the code.
Test - run a suite of tests, such as unit testing, integration, UI, smoke, or security tests. These tests aim to validate the behavior of the code. If this stage fails, then developers must correct it to prevent dysfunctional code from reaching the end-users.
Package - create an executable that contains the latest code and its dependencies. This is a runnable instance of the application that can be deployed to end-users.
Deploy - push the packaged application to one or more environments, such as sandbox, staging, and production. Usually, the sandbox and staging deployments are automatic, and the production deployment requires engineering validation and triggering.
