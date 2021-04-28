# TASk 1-Scenario 1c

## Examples for Docker



## Examples for Kubernetes


## Examples for jenkins ci/cd pipelines using
# - anisible

# - github
Integrate Jenkins with GitHub 
## Step 1:
In the jenkins server select Manage jenkins and in that plugin manager and under the available 
plugins search for GitHub. In that select Github Integration Plugin and download it. After 
downloading install and restart jenkins.
## Step 2:
And now in the jenkins home click on new items and enter a name for the item and select tthe 
type of project that we want to create.

# Examples for automated project setup on Azure DevOps Boards
To create an automated project on Azure devops first of all :
## Step 1:
Create an organization and in that create a project - for that give a unique project name and choose a visibility for the project.
now copy those commands to clipboard
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
![Screenshot (6)](https://user-images.githubusercontent.com/78786418/116392311-ebf36380-a83d-11eb-88d8-43b282d19561.png)


# Examples for automated project setup on Atlassian Stack
## Step 1: 
Create a project in JIRA
Open the jira website and login to your account, in that go to projects and click on create new project.
Select the type of project and give a unique name for the project. A key will be generated automatically.
A new project dashboard will appear, if you want to make any changes in the dashboard then go to configure dasshboard and change it.

## Step 2:
Create an issue
Click on the create option and select the project and in the issue type select the type of issue.
Give a summary for the issue and create it.

## Step 3:
Once you have created the issue you can go into backlogs and start the sprint.
By clicking on the issue we can assign the issue to a particlar person, set up a submition date etc.

## Step 4:
Steps to automate a project
click on project setting from the menu and in that choose the option automation in the window that appeares click on creat rule
in that we can specify the triggers so for a simpler use select create issues.Now save it
Next we can add new components to the rule, click new conditions and in the shown recomendations select Issue field conditions.
select the issue type and condition as equals and set the vaue as task and save it.
Nest step is to setup a new action and in the new recomentations select subtasks.
give the summary for the sub-task and add 2 more fields, and save it.

## Step 5:
Check if the automation works
to see if the automation is working go to your project and create a new issue-task and recheck in the automation window.
we can see that the job is stated and after soome time it is succeded.

Screenshots attached:

























 
