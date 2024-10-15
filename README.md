# AzurePipelines

It contains CI/CD pipelines for both AngularJs project and Dot net core

# AngularJS
For AngularJs CI pipeline :- 1. It contains Build job which will build the code and publish build as artifact.
                            2. It contains Test job which will run all the unit test and publish code coverage in artifact.

For AngularJs CD pipeline :- 1. It contains Download artifact job which will build made by CI pipeline using
                             pipeline-id.
                             2. It contains Deploy job which will deploy build in azure static web app using deplpyment-token.

# .Net Core

For .Net Core CI pipeline :- 1. It contains Build job which will build the image using docker file.
                             2. It contains Test job which will run all unit test and some scripts to publish code coverage.
                             3. It contains Push build job which will push the build in container registry.

For .Net Core CD pipeline :- 1. It contains deploy job which will take image from container registry and deploy it to 
                             container app 
