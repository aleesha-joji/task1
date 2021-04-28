# TASk 1-Scenario 1a

## Setup azure DevOps ci cd pipeline for app service application & deploy to dev, QA and production server. Add approver for every stage

Azure Pipelines provide a highly configurable and manageable pipeline for releases to multiple stages such as development, staging, QA, and production. it also offers the 
opportunity to implement gates and approvals at each specific stage.
 - Continuous deployment triggers
 - Adding stages
 - Adding pre-deployment approvals
 - Creating releases and monitoring deployments

## Step 1: 
In Azure DevOps create a new project and in that go to files to clone the existing repository. now copy those commands to the clipboard
in the required folder open cmd and perform the initial steps(git init, git add, and git commit)
after that paste the clone command and finally push it to the existing project

Now you have all the files in the Azure DevOps server
## Step 2: 
go to pipelines and click on new pipelines->use the classic editor->Azure Repos git click continue. On the next page in the featured section select ASP.NET core
and the next page in triggers enable continuous integration and save and queue the pipeline.
now the pipeline is running and succeded the job.

## Step 3:
Go to the Microsoft Azure portal and create a new resource group.
now create a new resource in the resource group. to create a resource select web app
select the subscription, resource group, give a specific name and give the runtime stack as .net 5 now review and create the resource.

## Step 4: 
Now go back to the Azure DevOps portal and in the pipelines select releases, in that create a new pipeline and in the features select Azure App Service deployment in this new release you can change the name and save it. next, go to tasks add subscription and authenticate it. next, select the resource group and save the stage
after this, you can see the new resource building and release.

## Step 5: 
finally, to add approvals in the releases click on the edit option, and in that, 
in each stage, there is an icon to add pre-deployment approvals. Click on that and set approvals. Again create a new release for the stage and during the creation, stage approve 
only then the release will be completed

## Step 6: 
Next is to add multi-stages to the pipeline, repeat steps 3,4, and 5.
And after you build and release everything delete all the resource groups and instances.



![Screenshot (5)](https://user-images.githubusercontent.com/78786418/116300956-210ba180-a7bd-11eb-86a4-8137b04887a0.png)
![Screenshot (6)](https://user-images.githubusercontent.com/78786418/116301037-35e83500-a7bd-11eb-8bfa-d134c99e0231.png)
![Screenshot (7)](https://user-images.githubusercontent.com/78786418/116301046-397bbc00-a7bd-11eb-81ca-fc20eea52538.png)

