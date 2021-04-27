# TASk 1-Scenario 1a

## Setup azure devops ci cd pipeline for app service application & deploy to dev,
qa and production server.Add approver for every stage

Azure Pipelines provide a highly configurable and manageable pipeline for releases to 
multiple stages such as development, staging, QA, and production. it also offers the 
opportunity to implement gates and approvals at each specific stage.
 - Continuous deployment triggers
 - Adding stages
 - Adding pre-deployment approvals
 - Creating releases and monitoring deployments

## Step 1: 
In azure devops create a new project and in that go to files in order to 
clone the existing repository. now copy those commands to clipboard
in the required folder open cmd and perform the initial steps(git init,git add, and git commit)
after that paste the clone command and finally push it to the existing project

Now you have all the files in the azure devops server
## Step 2: 
go to pipelines and click on new pipelines->use the classic editor->Azure repos git 
click continue. in the next page in the featured section select ASP.NET core
and in the next page in triggers enable continous integration and save and queue the pipeline.
now the pipeline is running and succeded the job.

## Step 3:
Go to microsoft azure portal and create a new resource group.
now create a new resource in the resource group. to create a resource select webb app
select the subscription, resource group, give a specific name and give the runtime stack 
as .net 5 now review and create the resource.

## Step 4: 
Now go back to azure devops portal and in the pipelines select releases, in that 
create a new pipeline and in the features select Azure App Service deployment 
in this new release you can change the name and save it. next go to tasks add subscription 
and autenticate it. next select the resource group and save the stage
after this you can see the new resource building and released.

## Step 5: 
finally in order to add approvals in the releases click on the edit option and in that 
in each stages there is an icon to add pre-deployment approvals. click on that and set 
approvals. Again create a new release for the stage and duing the creation stage give approval 
only then the release will be completed

## Step 6: 
Next is to add multi-stages to the pipeline, for that repeate step 3,4 and 5.
And after you build and releace everything delete all the resource groups and instances.

![Screenshot (5)](https://user-images.githubusercontent.com/78786418/116300956-210ba180-a7bd-11eb-86a4-8137b04887a0.png)
![Screenshot (6)](https://user-images.githubusercontent.com/78786418/116301037-35e83500-a7bd-11eb-8bfa-d134c99e0231.png)
![Screenshot (7)](https://user-images.githubusercontent.com/78786418/116301046-397bbc00-a7bd-11eb-81ca-fc20eea52538.png)

