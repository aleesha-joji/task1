# TASk 1-Scenario 1c

## *Examples for Docker*



## *Examples for Kubernetes*


## *Examples for jenkins ci/cd pipelines using*
# - anisible

# - github
Integrate Jenkins with GitHub 
## Step 1: 
In your Terminal, Start and enable Jenkins and docker
- systemctl start Jenkins
- systemctl enable Jenkins
- systemctl start docker
## Step 2: 
In your Jenkins console create your first job. Choose freestyle project with name and save
In the configuration section select SCM and you will add the git repo link and save it.
## Step 3: 
Then click on the Build option and choose to Execute shell
## Step 4: 
You will now write the shell module commands for the int phase and build the container. And after that create a new job. Next, Build it and choose to Execute the shell.
## Step 5: 
Write the shell commands again, Now it will verify the container files and the deployment will be done on port 8080, save it
## Step 6: 
Now, you will choose job 1 and configure it. And from the build actions, choose post-build and click on build other projects, give the name of the project to build after job 1 and then click save
## Step 7: 
Similarly, select and configure job 2. But in that from the build actions, choose post-build and click on build other projects. You will need to provide the name of the project to build after job 2 and then click save
## Step 8: 
let's create a pipeline, by adding to + sign. Now, select a build Pipeline view and add the name. Choose the Job 1 and save OK. RUN it and start the CICD process now
## Step 9:
After you build the job, To verify open the link in your browser localhost:8080/sample.text,

![image](https://user-images.githubusercontent.com/78786418/116462269-e4a47800-a886-11eb-8260-00b4a55c55f6.png)


# *Examples for automated project setup on Azure DevOps Boards*
To create an automated project on Azure DevOps first of all :
## Step 1:
Create an organization and in that create a project - for that give a unique project name and choose visibility for the project.
now copy those commands to the clipboard
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
finally to add approvals in the releases click on the edit option and that in each stage there is an icon to add pre-deployment approvals. Click on that and set approvals. Again create a new release for the stage and during the creation, stage approve 
only then the release will be completed

![Screenshot (6)](https://user-images.githubusercontent.com/78786418/116392311-ebf36380-a83d-11eb-88d8-43b282d19561.png)


# *Examples for automated project setup on Atlassian Stack*
## Step 1: 
Create a project in JIRA
Open the Jira website and log in to your account, in that go to projects and click on create a new project.
Select the type of project and give a unique name for the project. A key will be generated automatically.
A new project dashboard will appear, if you want to make any changes in the dashboard then go to configure a dashboard and change it.

## Step 2:
Create an issue
Click on the create option and select the project and in the issue type select the type of issue.
Give a summary of the issue and create it.

## Step 3:
Once you have created the issue you can go into backlogs and start the sprint.
By clicking on the issue we can assign the issue to a particular person, set up a submission date, etc.

## Step 4:
Steps to automate a project
click on project setting from the menu and in that choose the option automation in the window that appears click on creat rule
in that we can specify the triggers so for a simpler use select create issues. Now save it
Next, we can add new components to the rule, click new conditions, and in the shown recommendations select Issue field conditions.
select the issue type and condition as equals and set the value as task and save it.
Nest step is to set up a new action and in the new recommendations select subtasks.
give the summary for the sub-task and add 2 more fields, and save it.

## Step 5:
Check if the automation works
to see if the automation is working go to your project and create a new issue-task and recheck in the automation window.
we can see that the job is started and after some time it is succeded.

Screenshots attached:

![Screenshot (8)](https://user-images.githubusercontent.com/78786418/116462384-06056400-a887-11eb-938c-a95543dfa5ee.png)
![Screenshot (9)](https://user-images.githubusercontent.com/78786418/116462391-0998eb00-a887-11eb-9644-eace65cbadfc.png)




























 
