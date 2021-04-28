# TASk 1-Scenario 1c

## Examples for Docker



## Examples for Kubernetes


## Examples for jenkins ci/cd pipelines using
# - anisible

# - github
Integrate Jenkins with GitHub 
Step 1:
In the jenkins server select Manage jenkins and in that plugin manager and under the available 
plugins search for GitHub. In that select Github Integration Plugin and download it. After 
downloading install and restart jenkins.
Step 2:
And now in the jenkins home click on new items and enter a name for the item and select tthe 
type of project that we want to create.

## Examples for automated project setup on Azure DevOps Boards


## Examples for automated project setup on Atlassian Stack
# Step 1: 
Create a project in JIRA
Open the jira website and login to your account, in that go to projects and click on create new project.
Select the type of project and give a unique name for the project. A key will be generated automatically.
A new project dashboard will appear, if you want to make any changes in the dashboard then go to configure dasshboard and change it.

# Step 2:
Create an issue
Click on the create option and select the project and in the issue type select the type of issue.
Give a summary for the issue and create it.

# Step 3:
Once you have created the issue you can go into backlogs and start the sprint.
By clicking on the issue we can assign the issue to a particlar person, set up a submition date etc.

# Step 4:
Steps to automate a project
click on project setting from the menu and in that choose the option automation in the window that appeares click on creat rule
in that we can specify the triggers so for a simpler use select create issues.Now save it
Next we can add new components to the rule, click new conditions and in the shown recomendations select Issue field conditions.
select the issue type and condition as equals and set the vaue as task and save it.
Nest step is to setup a new action and in the new recomentations select subtasks.
give the summary for the sub-task and add 2 more fields, and save it.

# Step 5:
Check if the automation works
to see if the automation is working go to your project and create a new issue-task and recheck in the automation window.
we can see that the job is stated and after soome time it is succeded.

Screenshots attached:

























 