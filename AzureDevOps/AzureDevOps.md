**Azure DevOps**

**Introduction**

DevOps is combination of people, processes, and technologies to
continuously deliver valuable products and services that meet end-user
needs and business goals.

DevOps workflow walks through the following steps.

Plan \> Code \> Build \> Test \> Release \> Deploy \> Operate \> Monitor

**Primer to DevOps - Project lifecycle**

Waterfall - Model

Project planning \> Requirements\> Analysis\> Design\> Coding\>
Testing\> Deployment

Advantages

\- Clear demarcation between one phase and another

\- The requirement can be solidified up front

\- It gives the project manager a clear insight into aspects such as
delivery dates, cost estimates

Disadvantages

\- The customer might get to see the end product only at the end of the
entire lifecycle

\- Sudden changes in scope during the lifecycle should start from
analysis phase

\- Bugs in the testing phase

**Primer to DevOps - Agile methodology**

In software development, agile practices include requirements discovery
and solution improvement through the collaborative effort of
self-organizing and cross-functional teams with their customers/end
users, adaptive planning, evolutionary development, early delivery,
continual improvement and flexible responses to changes in requirements,
capacity and understanding of the problems to be solved.

Requirements \> Design \> Develop\> Test\> Deploy\> Review

**Primer to DevOps - Scrum process**

<img src="./images/f31be56f4d3eb7ad8f364e816007afbdc7942ab1.jpg"
style="width:6.40625in;height:3.47917in" />

\- Vision - The end application

\- User stories - The features and enhancements that user requires

\- Product backlog - The list of items to do based on user stories

\- Sprint backlog - Most important items selected from product backlog
for 2 weeks sprint

\- Sprint review- the team showcases what was done in the sprint. Here
the decision can be made as to whether the deliverable should be
promoted to production

\- Sprint retrospective- the team comes together to see what worked and
what did not work

**Primer to DevOps - Development and Operations**

When user requests a new feature to be added into production
application, the development team develops the feature and tests. But
operation team is hesitant to deploy the feature on to production unless
confirm the the feature is fully tested in term of security,
vulnerabilities.

**Primer to DevOps - About DevOps**

\- The entire purpose of DevOps is to ensure that developers and IT
operation work in collaboration during entire application lifecycle

\- Both team collaborates at the beginning of the project. Meeting that
are held with stakeholders normally have the developers and operation
teams

\- Automation is a key aspects.

\- Faster delivery of application features

\- Adoption of the right tools

**Configure processes and communication**

**Project**

\- This provides a place for storing the source code. Here users can
plan, track progress and collaborate.

\- When you create a project, a team of the same name as the project is
created.

<https://dev.azure.com/nibhathaka/AgileProjects>

**Organization**

\- This can contain a group of related projects

\- For example, you could have an organization for each business units

\- Each organization gets its own free tier of services(up to five users
for each service type)

\- Choose what you need to complement existing workflow

<https://dev.azure.com/nibhathaka/>

**Creating user stories**

\- Create a work item - epic as parent for the application that develops

\- Create work items - user story as child for the features that need to
be encapsulated into the application

**Azure boards**

Kanban - This is framework available that can be used to implement agile
and DevOps. It use to visualize the work items.

**Work item process**

Process can be chose out of followings.

\- Basic - uses Issues, Tasks, and Epics to track work.

\- Agile - to track user stories and (optionally) bugs on the Kanban

\- Scrum - track product backlog items (PBIs) and bugs on the Kanban
board, or break PBIs and bugs down into tasks on the taskboard.

\- CMMI - to track requirements, change requests, risks, and reviews.

**Adding tasks to user stories**

Add tasks that need to accomplish user stories in backlog. The tasks
create show in work items.

Then user stories along with task should be assigned to iteration which
is called sprint and set date for 2 weeks on sprints.

**Creating users**

\- Can add users to Azure DevOps organization

\- The users can be Microsoft accounts or GitHub usernames

\- The users can then be assigned to the required project

\- Then user can see all items in the project assigned

**Access levels**

Basic - This provides most of the features within Azure DevOps which
excludes Azure Test Plans

Basic + Test Plans - This gives access to Basic Plan + Test Plans

Stakeholder - This is a free access but has limitations. Limited access
to Azure Boards and Pipelines. No access to code repositories.

Visual studio - This depends on the Visual Studio subscription assigned
to the user

**Using dashboard**

Can create dashboard using in built widgets to display the progress of
tasks and performance of the team.

***Widgets***

Following are the project metrics that can show in dashboards.

Burndown chart - these chart focus on the remaining work within a
specified period of time

Cycle time - This defines the time taken to close a work item after work
on it has started

Lead time - This defines the time taken to close a work item after it
has created

Velocity - This tracks the team’s capacity to deliver work sprint after
sprint

<img src="./images/01dc1cfce11c20f898e36da493fe5f861045ffc1.png"
title="The following diagram illustrates how lead time differs from cycle time. I 
calculated from work item creation to entering a completed state. Cycle 
from first entering an In Progress or Resolved state category to entering 
category. To understand how workflow states map to state categories, se 
states and state categories are used in Backlogs and Boards. 
In Progress Reølved 
Work Item" style="width:5.4375in;height:3.38542in" />

**Using queries**

Using queries on boards allow you to query work items based on different
conditions that combined. It can be shared query for others to use.

We can visualize the query that saved by creating chart.

Only chart generated from shared query can be added into dashboard where
others users can view shared query and chart on dashboard.

**Understanding permissions**

In build security group with permission level defined are available at
project and organization level.

**Query permissions**

This is about query based permissions.

\- All users except those that are only assigned to the Readers group
can create and edit their own queries.

\- They can save their queries under My queries

\- Member of the Project administrator groups can create and edit
queries and folders under Shared Queries

\- We can give certain permission to specific user on Shared queries
using security settings.

**Dashboard permissions**

\- Dashboards are viewable by all members that are part of the Project
valid Users group

\- Members of the Project Administrators group can set the default
dashboard permissions for the teams

\- To add, edit and manage a team dashboard, you must have Basic access
or greater

**Wiki**

\- A DevOps project can have a wiki

\- The wiki can be used to share information with the team so that they
can understand and contribute to the project

\- The project wiki uses a Git repository at the back-end

\- You need to have at least the Basic access to create and modify a
wiki

\- Members who are part of the Contributors security group can add and
edit wiki pages

**Delivery plans**

\- The way of visualizing your work

\- Create a delivery plan by specifying project and backlog where you
can see the progress of project

**Integration with Microsoft Teams**

\- Create Microsoft account and sign in with the account

\- Create team in Microsoft Teams

\- Turn on third-party application access via OAuth in Organization
settings \> Security \> Policies

\- Add permission to an user in project administrator security group at
project settings

\- Add the Azure boards app in Teams app and link the project with
project URL

-You can link your Azure Boards project with the Teams channel via the
@azure boards link command.

**Create scrum project**

\- It has work item - feature at same level as epic

\- Product backlog item instead of user stories

\- Task is part of product backlog

**Design and implement source control**

**Source control**

\- Helps to maintain different version of file where source code
includes

\- Also help us revert back to prior version

**Git**

\- Most commonly used version control system because of its distributed
nature

\- Subversion client is a source control app where it allows to checkout
files required, make changes to the code, check in the code with the
required changes on to the server

\- Thus another developer can make changes to the code in file on the
server

\- The drawback of this sort of centralized system is that developers
checkout the file required when the server is offline. This is why we
need distributed system which is called Git

\- Developers get their own copy of application code through Git client
and make changes as required. Git maintains version when it comes to the
application code

\- Git has better overall performance and easily manage aspects like
creating branches

**install Git**

\- Install git client on any OS

\- Select use of credential manager to manage GitHub access through it

git init; initialize an empty git repository

\- Once you initialize git directory, the files in the directory will be
added to working area. It shows by adding an annotation in front of name
of the file

git config - -global user.name “Nibhath”

git config - -global user.email “<nibahth512@gmail.com>” ; make global
config

**Adding to git repository**

\- When create an empty git repository, it creates .git folder which is
like local database within git itself

\- It maintains the entire history of changes

\- Contains information on the commits, remote repository address

\- In your working directory, there is a hidden folder which is called
.git. That is flat file database which track version of files in the
folder

git add . ; add all files in working directory on to staging area, you
can see annotation M

git status ; status of the current directory

\- Git software manages moving files from working area\> staging area\>
git repository

git commit -m “This is the initial commit” ; commit files to git
repository from staging area along with meaningful message

\- Then the files are tracked by git repository and staging area which
cannot be visible

**Making changes to a file**

\- You can make changes in file, then add file into staging area and
commit to git repository

\- Staging area allows to review changes before committing to git
repository. We can unstage file at anytime

git - -version ; check version

git log ; show entire history that changes made to git repository along
with message you specified, commit ID, author, date and time

git checkout \<commit number\> ; checkout any version of file back and
forth

git log - -all ; to check all history of commits after performing
checkout

**Un-staging a file**

\- When you add a file to staging area, it shows as HEAD detached

git checkout main ; attach to main branch if the file detaches from main
branch

git rm - -cached file.txt ; untrack the file, you can see annotation U

**Git Branches**

\- When a Business Unit comes with a new feature or bug fix, branches
will help to segregate the changes make on to main code that the change
is either feature or bug fix

\- If new feature needs to be developed, a new branch is created out of
your main code

\- Whatever is your code at that point in time, its time a copy is being
made, then you can start adding or changing code to add that new feature
or bug fix has a new feature branch, then merge feature branch with the
main branch

\- Creating new branch is apt of deviating the main branch at point in
time

**Working with branches**

git checkout -b FeatureA ; create a new branch and switch to that branch

**Merging the branches**

\- Merging a feature branch with main branch makes both branches have
same set of files and changes

\- The default merge is fast-forward

\- git log shows head is at main and feature branches

\- Merge feature branch from standing on main branch

git checkout main ; check out to main branch

git merge FeatureA ; merge feature branch with main branch

**GitHub**

**Using a remote repository**

\- Way to store your application code in centralized location instead
using git software or local server

\- GitHub and Azure Repos within Azure DevOps services are to use
hosting git repositories

The developers use git client tool

\- Clone application code from the remote repository

\- Make changes to local repository

\- Merge the changes from the local to the remote repository

First create remote repository in GitHub.

git remote add origin
<https://github.com/techsup/application/application.git> ; add remote
repository as an origin to publish files

git push -u origin main ; push all application code file in the main
branch to remote repository

After running this command, it pops up option to sign in with browser or
code to GitHub where you can use GitCredentialManager by authorizing to
manage access. Once authorization is complete, the files in local
repository will be published to remote repository.

**Committing changes to GitHub**

\- Changes make on file are committed to local repository

\- Check git log to verify origin is pointed to main branch

\- Run git push command to commit changes to remote repository

\- Thus, changes on feature branch can be directly merged to main branch
on remote repository using git pull

**Using Visual Studio**

\- Start simple .NET core web app project using visual studio

\- Integrate source codes with git repository where it initializes local
repository to commit changes and push changes remote GitHub repository
created

\- Whereby GitHub repository will be created by Visual Studio API

**Publishing code from Visual Studio**

\- To collaborate with source code commits to GitHub repository, GitHub
organization should be created and add users who are allowed to
collaborate with source code. The user who are going to collaborate with
code should have GitHub account

\- The organization created can be selected as owner when you create git
repository on visual studio and push changes in project to organization

**Clone the repository as another user**

\- Invite users into organization where users can accept the invitation
via email or join to organization on GitHub itself

\- The user invited can clone repository onto Visual Studio 2022 from
GitHub and the can start making changes on application code

\- Specify the path to clone and browse the repository by authenticating
from GitHub account of the user

\- In order to let users to write permission on the project, admin
should provide read permission for user at organization level

**Create merge request**

\- When a change on GitHub repo and then local git repo, the first
change should be pulled prior to subsequent change to be merged with
main branch using Visual studio and push the change to GitHub repo

**Different merge process**

A simple fast-forward merge happened wherein the main branch just
pointed to the latest commit of the feature branch.

git log - -graph ; can see changes in graph basis

***Ort merge***

When we do change on to main and feature branch at same time and merge
together, where 3 commits happen on changes in each branch and for the
merge.

***Squash merge***

This helps to reduce number of commit messages that shows in git logs
after making changes onto each branch and making merge. It shows last
commit made as head of main branch.

git merge - -squash FeatureA ; merge branches with squash strategy

**Creating a branch on GitHub**

\- Create new feature branch

\- Make change and commit

\- Create pull request

\- Then merge pull request using either squash or rebase to main branch

**Creating branch on Visual Studio**

It creates branch on local git repository and could publish branch to
GitHub.

\- Create a feature branch based on main, select checkout to branch

\- Make change on file in feature branch

\- Commit all and push from visual studio

\- Create new pull request on branch created on GitHub

\- It shows there is a conflict to be resolved, the resolve conflict

\- Remove the old conflict from file, then resolve and commit merge

\- Merge pull request and confirm the merge with main branch

**Adding a branch protection rule in GitHub**

\- Add branch protection rule in settings section by specifying name of
the branch

\- When an user make changes on the branch that you added protection
rule, it shows user to the branch is protected

\- If require pull request before merging, the user will need to create
new branch for the change and to create pull request

\- From main branch, review and approve pull request and merge pull
request, confirm merge

**Tagging git**

\- It can be used to specify which commit is important in the repository

\- Can mark release points with the use of tags

\- Two types of tags - lightweight and annotated

\- Lightweight tag is just a pointer to a specific commit

\- Annotated tags store as full objects in the Git database. These are
checksummed, they contain the tagged name, the email and date, have
message. It can also be signed and verified with GNU Privacy Guard

git tag -a “V1.0” -m “This is version 1” ; tag will be added to previous
commit

git tag ; show tags contain in main branch

git show v1.0 ; show details of specific commit that tags is attached

git maintenance and recovery

git gc - -auto ; stands for garbage collect. This gathers all the loose
objects and place them in packfiles. It removes objects that aren’t
reachable from any commit that few months old

git prune - -expire now ; remove stale objects

**Large files in Git**

\- Git repository has small text file instead of binary files

\- Need to install Git LFS to mange large file in git

**Branching strategies**

\- Always maintain a high quality for main branch

\- Contain the working copy of your production code

\- Create feature branches for features and bug fixes

\- Use pull requests to merge feature branches into main branch

\- Don’t create long feature branch, keep them short-lived. Delete
feature if it is no longer required

\- You also need to ensure that your feature branch is merged onto both
your release and main branches

\- Here you need to maintain your release and main branches as well

\- If multiple customer different features in the application, maintain
different release branch for the customers upon main branch

**Azure Repos**

\- When we create repository in Azure Repos, it show origin URL to add
git local repo to Azure Repos

\- Azure Repos is similar to GitHub repository

git remote add origin
<https://nibhathaka@dev.azure.com/nibhathaka/AgileProject/_git/AgileProject>
; add remote repository has an origin

git push -u origin all ; push all application code file in the main
branch to remote repository. Then it is popping up git credential
manager to connect Azure Repos with Azure DevOps account

**Azure Repos - Branches**

git checkout -b FeatureB ; create a feature branch and switch to branch

Make changes on files in the branch and commit.

git push -u origin featureB ; push changes on feature branch to remote
repository

**Azure Repos - Pull request**

\- To merge feature branch to main branch using Azure Repos, we use pull
request

\- A title, reviewer, work items to link and tags can be added

\- It shows no merge conflict, then complete pull request choosing merge
strategy which have options such as deleting feature branch

**Azure Repos - Importing GitHub repos**

\- Select ‘Import repository’ from the project in Azure devops, specify
a name, clone URL of GitHub repository, authentication(username/password
or Personal Access Token)

\- For PAT, GitHub settings \> developer settings \> Personal Access
Tokens - generate PAT with required scope

\- Import repository from GitHub to Azure Repos by authenticating using
PAT

**Azure Repos - Branch policy**

\- Specify minimum number of reviewers for branch, link merge types,
comment resolution on branch policy in required branch

\- Do the change on files in the branch and create pull request to merge
with main branch

\- Have an option to allow merge branch only if linked work items is in
place

**Azure Repos - Branch security**

\- Permissions for users and groups can be managed at the branches and
repositories

**gitignore file**

\- The files that exclude from version control in working directory I.e
build of the code, binary files such as DLL

\- Create the files that need to ignore and make change, then it shows
untracked. The create .gitignore file and enter the name of file that
needs to ignore and save

**Azure Repos - Publishing from Visual Studio**

\- Create a project and then Git repository specifying local path of
local git repository, account, organization, project on Azure DevOps

Deviation-Azure pipeline

When you create Azure pipeline and run pipeline YAML file, it pops up
failed job as following error.

“No hosted parallelism has been purchased or granted. To request a free
parallelism grant, please fill out the following form
<https://aka.ms/azpiplines-parallelism-request>”

Need to fill the form and it will take couple of day to grant approval.

**Azure Repos - Visual Studio- cloning repository**

\- Clone repository specifying local path, authenticated Azure Repos,
then select the repo to clone

\- Make change on the files, commit all and push to Azure Repos

**Azure Repos integration with Microsoft Teams**

\- To subscribe Azure Repos with Teams, The user who connects Teams with
Azure Repos should member in the project administrator in Azure DevOps
project

\- Add the Azure Repos app from Teams, use following command to
subscribe

@Azure Repos signin

@Azure Repos subscribe \< project URL or repository URL\>

You have added the Azure Repos app to your Slack workspace. You now need
to monitor the Git repositories within the Azure DevOps project.

/azrepos subscribe <https://dev.azure.com/techsup1000/app-project>

**Azure Boards integration with GitHub**

\- Integrate GitHub with Azure boards in order to link work items with
GitHub pull request

\- Use GitHub marketplace to find Azure Boards app, then connect

\- Add comment on pull request with ID of work items in Azure Boards to
link with

Work items task - TASK 18

Comment - AB \#18

**Team Foundation Version Control(TFVC)**

\- This is a centralized version control tool that was developed by
Microsoft

\- It’s different from Git which is a distributed version control tool

\- With TFVC, a team member has only one version of each file on their
local machine

\- The historical data for the files is held on the server

\- Before developers can make changes to a file, they need to first
check out the file from the server

\- When it comes to each file, you can apply permissions at the file
level, but where the permissions can be set on the repository or branch
level

\- Create a project with version control set to Teams Foundation Version
Control

\- In VS 2022, select visual studio team foundation server as plug-in
selection in tool \>option

\- Select Team explorer, then mange connection to connect with Team
foundation project in Azure DevOps

\- Map it to local path

\- Add source control and check in all included change into team
foundation repository.

**Public and private projects**

\- By default, public project is disabled in organization settings

\- In public projects, users are not signed into the service and have
read-only access

\- In private projects,it requires users to be granted access to the
project and signed in to access the services

\- Public GitHub repository is also functioned in same way

**Cherry picking changes**

\- To choose the commits that can be copied from one branch to another

\- The specific commit that has been applied to a feature branch can be
picked to main branch by using the specific commit number of feature
branch

git checkout Feature ; switch to feature branch

git log ; get specific commit number of the change

git checkout main; switch to main branch

git cherry-pick \< commit number \> ; get main branch head to latest
commit number specified

**Design and implement build pipeline**

**Continuous Integration**

Automatically building and testing code every time a team member commits
code changes to version control

In our local machine,

\- In visual studio, when we run an application, a build of the
application is conducted first

\- The build tool builds the project and the dependencies into a set of
binaries

\- The binaries can then run on the target machine with the help of
runtime

Though, developers use programming languages to develop an application
such as Java, C#, the machine only understands how to run binary
instructions.

Let see you develop .NET application,

\- Developers code an application using the .NET 6.0 SDK

\- The local machine needs to have .NET runtime installed to run
application that would take build of the code, then incorporate with
binary instructions

**Build process**

\- Create a project with ASP.NET Core web app where it is available .NET
SDK web

\- Build the application from Visual Studio which shows output of build

**Publish process**

\- After building the app, it can publish to target location which may
be local folder, Azure, container registry

\- If the target location is a local, publish the built code and copy
the code published to target machine that run required runtime

Team 1 works for bug fixes and team 2 works for new features. They work
through separate feature branches and make changes to main branch of the
repository.

\- Automation is key

Changed and commit the code to repository\> The code needs to be built
\> The code needs to be tested

This is the concept behind the continuous integration.

**Azure Pipeline**

\- Automation - Build and test your code projects

\- Functionality- you can use Azure pipelines for both continuous
integration and continuous delivery

\- Languages - It has support for languages- Python, Java, PHP, Ruby, C#

\- Deployment- You can deploy your application to multiple targets or
environments

Using Azure pipelines

\- You can define your pipeline in YAML syntax which human readable data
serialization language

\- A file called **azure-piplelines.yml** will be created and version
controlled along with your code with git repository with Azure Repos

\- This helps to easily identify changes in the pipeline that could
break the deployment

\- The classic interface gives you a graphical interface

\- You can the define your pipelines with the use of this interface

**Creating pipelines**

\- Check main branch in a repository in Azure Repos to create Azure
pipeline

\- Create pipeline \> select where remote repository is( Azure Repos
Git, Bitbucket cloud, GitHub) \> select the repository that the code is
hosted on\> select underlying programming language( ASP.NET, ASP.NET
Core, Universal Windows Platform) \> then it gives YAML definition of
build pipeline.

- It has a trigger where the build pipeline will be triggered whenever
  changes commit to main branch \> save and run

- The YAML code will have version control along with the application
  code

- Once run Azure pipeline, it initialize a job. Each pipeline has runs
  as versions.

- It starts to go through various tasks that has been defined in that
  particular pipeline

1\. initialize the job as part of the build

2\. download the required tasks

3\. Checkout code from main branch in the repository

4\. Do VSBuild task which build particular .NET project

***Terminology in Azure build pipeline***

trigger - it triggers build pipeline whenever make change on to main
branch

Pool - It shows vmImage that use to spin up VM. It is called Microsoft
hosted agent. These are VM that is spun up during each new job of the
pipeline. The code of project is copied onto the VM from repository and
build the code. After the job is finished running, Azure DevOps destroys
the VM.

Further, it has functionality to have own hosted agent. The agent has
tools that require to build your applications.

When you build the project on local machine, Visual Studio internally
use of an MS build tool to build the project into required binary files.

Variables - that are name value pairs to reuse across the script

Steps - series of tasks that needs to carry out. All of the tasks are
executed on the VM that spun up

1\. Installation of NuGet tools - It uses to restore NuGet based
packages that use as part of the project. They send request to Azure
DevOps to perform functionality based on the programming language

2\. Restore the solution which is part of the repository- The repository
has solution file .sln extension.

3\. Task for VSBuild - That is used to build your entire project. Azure
DevOps creates a script to run these tasks on the VM. (Use .NET Core CLI
task to build and publish .NET Core project)

Azure DevOps has inbuilt tasks in order to add functionalities into
Azure pipeline conveniently

**Triggering pipelines**

Once make change on main branch in the repository and commit the change,
the Azure pipeline is automatically triggered to build another version
of build.

**Microsoft hosted agent**

The Azure Pipelines agent pool offers several VM images to choose from.
Mostly YAML VM image label is **windows-latest** which has Windows
Server 2022 with Visual Studio 2022. Thus, there are several VM image
with different Windows versions, Linux distribution such as Ubuntu and
macOS.

With the VM image, it has software included such as language and
runtime(Bash, Go, Kotlin, Perl, PHP, Python, Ruby) and package
management(NPM, NuGet, pip, Helm), tools(Docker, Git, Kubectl, OpenSSL),
environment variables.

-The entire pipeline is making use of a Microsoft hosted agent. That’s
the simplest way to run the pipeline.

-A fresh VM is created for each new job of the pipeline. After the job
is run, the VM is discarded

.NET core webapp can be built on either Windows or Linux VM. If you are
using Ubuntu image, it may occur an error if .NET Core that requires is
not placed on the agent. In that case, add a ***.NET Core*** task with
the version onto YAML pipeline.

The Microsoft hosted agent purges builds when VMs are discarded.

**Self-hosted agent**

The biggest advantage is that all maintenance, upgrades and security
patches are handled by Microsoft when it comes to the Microsoft hosted
agents.

Self-hosted agent may needs when;

\- There may have use case to create your own agent.

\- You want to have builds to store on a machine.

\- Have custom software installed and third party components requires
for your application

\- When you want to store builds in another location like on-premise
machine after the build

**Deploying self-hosted agent**

\- Create a VM in Azure

-Turn off IE Enhanced Security Configuration

\- Install git as tool

-Install .NET SDK 6.0 or 8.0

**Registering the self-hosted agent with Azure DevOps**

\- Use the VM as self-hosted agent and run pipeline to create build
using self-hosted agent

\- Sign in to Azure DevOps account from the VM itself. Then generate and
copy a Personal Access Token in profile settings to authorize
self-hosted agent with Azure DevOps

\- To generate PAT, you should specify name, organization, expiration,
scope of access(Full access or custom defined), scopes(Work items, Code,
Build, Release, Test management, Packaging and more) where agent pool is
to be enabled with Read and manage access and get copy the PAT once it
prompts(The value of PAT will not be available at later point in time)

\- Download a new agent from default agent pools in organization
settings in order to run pipeline jobs

<img src="./images/70d07dd4004599787534e428a496842edac783d5.png"
style="width:4.58333in;height:4.83333in" />

\- Make a directory in C drive. Copy downloaded file into directory and
extract the file

\- Navigate directory and run the config file : ./config.cmd on Windows
PowerShell which require Azure DevOps server
URL(https://dev.azure.com/nibhathaka) and PAT that generated to connect
with Azure DevOps

\- Register agent by specifying agent pool, agent name, path of work
folder created separately on C drive(C:\work), run agent as service,
then the agent registered can be appeared in list of default agent pool.
But it would be Idle state at first and become online after few minutes

\- Now the self hosted agent is part of your Azure pipeline

**Running pipeline**

\- Specify the name of the agent pool(name:\<agent pool name\>) that
self-hosted agent is registered by replacing the VM image and save the
pipeline with commit message which will start running the pipeline job

\- It will show that this pipeline needs permission to access a resource
before this run can continue. Once permit, the permission will use queue
‘Default’ for all waiting and future runs of this pipeline

\- Running time for pipeline jobs take bit longer time as all commands
need to run self-hosted agent remotely

**Exploring the work folder**

\- In the work folder, there is a folder structure adopted by Azure
pipeline when it comes onto pipeline itself

\- In c:\work\1\s, it has source code which is actual source code that
is picked up from Azure Repos

\- The pipeline first needs to download the code which has project files
to the VM, and then build the code accordingly

\- In the work folder, we can’t find the location where the build is
because the code we build has not been published.

\- In Visual Studio, we publish the build once the build is made from
the project code.

\- Likewise, we need to add one more task into Azure pipeline to publish
the build after task for creating build and run the pipeline

\- task: DotNetCoreCLI@2

inputs:

command: publish

publishWebProjects: True

arguments: '--configuration \$(BuildConfiguration) --output
\$(Build.ArtifactStagingDirectory)'

zipAfterPublish: True

\- The build published is stored in c:\work\1\a as zipped file which is
special directory location Build.ArtifactStagingDirectory that output is
directed in pipeline

\- By default, build will be zipped after publish where zipAfterPublish:
true

\* If you are using self-hosted agent, you don't need to use Use .NET
Core task that for installing .NET SDK and NuGetToolInstaller for use
external NuGet packages on Azure pipeline

\****Build.ArtifactStagingDirectory*** is a predefined variable that map
the build published to the path - c:\work\1\a

In the pipeline, you can see amount of time spent for each run relative
to each other

<img src="./images/56e524890e28effcb99b4bc7311de266f6f19249.png"
style="width:6in;height:0.9375in" />

Azure pipelines get version control along with code repository in Azure
Repos

<img src="./images/0b79b493606535ed89ba8793a5c866c3656e88a5.png"
style="width:6.13542in;height:1.96875in" />

**Security at every stage**

\- Security needs to be embedded at every possible stage in your
lifecycle

\- For web applications, there are possible threats that needs to
mitigate in planning and development stages

\- Using security plug-in in the integrated development environment,
they can look for potential issues within the code at every stages such
as planning, development

\- Conduct peer reviews on the code and provide advise for improvement

\- Adhere with coding standards that the organization maintains

\- In continuous integration stage, you have tests embedded within the
pipeline as example unit tests in place

\- Use static code analyzers that can look at possible issue in the code

\- In continuous deployment, perform load testing, penetration testing,
infrastructure scanning at test or staging environments

Static code analysis - You can analyze your source code without
executing it(during CI phase), detect security weaknesses before
integrate your code to the main source code. Static code analysis tools
in the IDE provide the first line of defense to help ensure that
security vulnerabilities are not introduced into the CI/CD process.

Penetration testing- It typically perform after CI/CD processes,
identify vulnerabilities and assess the security, simulating
real-attack.

Dynamic code analysis, unlike Static code analysis this evaluates the
app during runtime (not during CI)

Threat modeling, identifies potential threats and vulnerabilities for
the app during design and planning phase.

**Using the Mend Bolt tool (formerly WhiteSource) - Setup**

\- An open source software security and compliance management tool

\- It integrates with the Azure DevOps set of tools, in the build
pipelines

\- Check for any sort of security vulnerabilities, licensing issues

\- Developers might install external packages and external open source
libraries which may be developed by external parties where those
packages and libraries may have security loopholes by not considering
security best practices.

\- The external packages and libraries may come with the requirements of
licenses. You may install packages without considering license
requirement. Hence the mend bolt tool is capable to identify license
requirement, potential vulnerabilities and outdated libraries

\- Get Mend Bolt extension to be installed through Azure DevOps
organization settings (Organization settings\> Extension \> Browse
marketplace)

\- To use Mend Bolt tool, you have to integrate your Azure DevOps
account with Microsoft Entra ID

\- Switch to default directory and create new Azure DevOps organization
that connect to Microsoft Entra ID

\- Install Mend Bolt extension as part of new organization

-Navigate organization settings \> Extensions \> Mend

-Add your information to create free account in Mend Bolt to activate
extension

**Using the Mend Bold tool - Usage**

\- Create .NET Core project in Visual Studio

-Create git repository in Azure Repos from .NET Core app to Azure DevOps
organization

\- Create a build pipeline from git repository pushed and add ***Mend
Bolt*** task into YAML pipeline using show assistant

\- Mend bold extension generates open source risk report once build
pipeline job is completed. It shows status of security vulnerabilities,
license risks, inventory that incorporate on libraries, packages

\- task: WhiteSource@21

inputs:

cwd: '\$(System.DefaultWorkingDirectory)'

<img src="./images/485e132a8c268de930d825e2df86620e95dd90ec.png"
style="width:6.79167in;height:2.90625in" />

\- To check with more result, install ***newtonsoft.json*** package into
the project (Tools \> NuGet Package Manager\> Manage NuGet Packages for
solution )

-Commit all git changes to push the change to Azure Repos

\- Since Azure-pipeline.yaml file has now been added by Azure build
pipeline onto depository, hence there is conflict so that change has to
be pulled from Azure Repos and then push again.

-Commit all triggers the Azure pipeline and show the results of Mend
bolt after new package is added

<img src="./images/6084d8405ad636f2b2ea29069318f527e1fd4c55.png"
style="width:7in;height:3.16667in" />

**Adding unit tests as part of local project**

To have unit test in place as part of build pipeline, need to define
unit test as part of the code where we use unit test as separate project
within visual studio solution.

\- Clone a repository from Azure repos to local path into local machine

\- Select solution file from solution explorer and choose to add new
test project

\- Then test project will be added as part of main code. We add ***xUnit
Test project*** within main project.

\- When Run all test from Visual Studio , it creates a build first and
then run test locally

**Running unit tests in the pipeline**

\- Add a ***test*** task into pipeline for unit test where we should use
name of test project we created within main project and commit the
change which trigger running the pipeline

trigger:

\- main

pool:

vmImage: 'ubuntu-latest'

variables:

solution: '\*\*/\*.sln'

buildPlatform: 'Any CPU'

buildConfiguration: 'Release'

steps:

\- task: UseDotNet@2

displayName: Install .NET 6

inputs:

packageType: 'sdk'

version: 6.x

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: DotNetCoreCLI@2

inputs:

command: test

projects: '\*\*/webtest.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- Commit all and push the test project added into Azure Repos which
start to run the pipeline again

\- It will start syncing changes by pulling and pushing the changes into
Azure Repos

-After completing the pipeline runs, it creates Tests pane which
includes test result such as total test, pass percentage, run duration

**Code coverage- Adding unit test**

\- With code coverage, we can measure ***how much of your actual
application code is being tested by the unit test***

\- Add a module folder into main code and create a function class in the
module

-Add new method based on function class into test project

\- Create test on the solution for the function, run all test to verify
the test locally. Then push the code to Azure Repos that will trigger
the pipeline with test task and show the test results

**Code coverage - Implementation**

\- We can add task for code coverage tool(Cobertura or JaCoCo) and code
coverage results into build pipeline

\- This is to check whether your unit test is testing all parts of your
code within the main application code

-Install ***coverlet.msbuild*** NuGet package library on the test
project, build solution and promote it to Azure Repos

-Add ***.NET Core CLI*** task for restore into build pipeline

-Add argument as CollectCoverage=true, CoverletOutputFormat=cobetura
into test task in build pipeline

-Use ***Publish Code Coverage Results*** task in a build pipeline to
publish code coverage results to Azure Pipelines

JaCoCo is a free code coverage library for Java, which has been created
by the EclEmma team based on the lessons learned from using and
integration existing libraries for many years. Use Publish Code Coverage
Results task in a build pipeline to publish code coverage results to
Azure Pipelines or TFS, which were produced by a build in Cobertura or
JaCoCo format.

-Commit all and pull changes on main project to trigger the build
pipeline

-Run the build pipeline and complete which shows code coverage tab, you
can see covered lines, coverable lines, line coverage, the classes
covered by unit test

trigger:

\- main

pool:

vmImage: 'ubuntu-latest'

variables:

solution: '\*\*/\*.sln'

buildPlatform: 'Any CPU'

buildConfiguration: 'Release'

steps:

\- task: UseDotNet@2

displayName: Install .NET 6

inputs:

packageType: 'sdk'

version: 6.x

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: DotNetCoreCLI@2

inputs:

command: 'restore'

projects: '\*\*/\*.csproj'

\- task: DotNetCoreCLI@2

inputs:

command: test

projects: '\*\*/webtest.csproj'

arguments: '/p:CollectCoverage=true /p:CoverletOutputFormat=cobertura
/p:CoverletOutput=./MyCoverage/'

publishTestResults: true

\- task: PublishCodeCoverageResults@1

displayName: 'Publish Code Coverage Results'

inputs:

codeCoverageTool: 'Cobertura'

summaryFileLocation:
'\$(Build.SourcesDirectory)/\*\*/MyCoverage/coverage.cobertura.xml'

**Azure pipeline- GitHub repository**

\- Azure pipeline can pickup code from GitHub repository so that the
pipeline should authorize with GitHub repository

\- There are three authentication types for granting Azure pipelines to
access GitHub repositories.

Personal Access Token - a personal GitHub identity. No GitHub checks

OAuth - a personal GitHub identity which pass secret. No GitHub checks

GitHub app -You can install Azure pipeline as an app in GitHub account
so that the pipeline can run with Azure pipeline identity. GitHub check
is available.

\- When create a new Azure pipeline with GitHub repository, it requires
to authorize with OAuth secret or GitHub app wherein GitHub will be
linked with Azure DevOps

\- In the selected repository settings in GitHub, you can find installed
GitHub app in Third party access section at organization level

**GitHub status badge**

\- The status of the pipeline runs can be reflected onto GitHub
repository using GitHub status badge

\- Copy ***sample markdown*** from status badge in the pipeline and
paste into readme file in the GitHub repository, the commit new file to
main branch which trigger new run in the pipeline

\- If you need to see reflection correctly, uncheck ***disable anonymous
access to badges*** at organizations and project settings level

<img src="./images/af32f8991101fdd37ae31c3f0dd012b0809ebb23.png"
style="width:5.5625in;height:3.59375in" />

**Azure pipeline-Classic Editor**

\- To create connection between Azure DevOps and GitHub, we can create
personal access token classic (GitHub account\>settings\>Developer
settings\> Personal access token \> generate new token(classic)- scopes
admin:repo hook, [read:user](http://read:user/), user:email)

-Create new service connection to GitHub (Project settings\> Service
connections\>New service connection \> select connection type -GitHub\>
Authentication method- Personal access token\> Paste the PAT generated
from GitHub\> give service connection name\> check grant access
permission to all pipeline\> verify and save )

\- Azure pipeline creates apart from YAML based build pipeline file are
known as classic editor such as ***other Git***

-A new service connection can be authorized using a Personal access
token generated from other end git repository or you can select existing
service connection

\- After specifying specs such as source of the code(GitHub), select the
repository and branch, featured type of the project(ASP.NET core
framework), you need to set up the tasks in the job using GUI where
agent pool, agent specification, branch, commit message must be
specified, the save and run. You can add and removed task as you need
and make change on the attribute in the tasks.

<img src="./images/cc05f29c92014fd4777837e57e7f03535cedc96a.png"
style="width:4.375in;height:5.02083in" />

\- In Azure pipeline - classic editor, you can add variable, triggers
where you can enable continuous integration in order to trigger the run
of build pipeline automatically once make change and commit onto GitHub
repository

**Using SonarCloud**

\- SonarQube and SonarCloud are used to improve source code quality and
security which provides solution for static code analysis

\- We can integrate SonarCloud with Azure DevOps by logging in
SonarCloud(sonarcloud.io) through Azure DevOps

\- Create a new project manually and then create an organization with
name, key, choose a plan in SonarCloud. After creating organization, add
project key and display name, public, set up

-Generate a token from SonarCloud(SonarCloud account \> Security \>
Generate token \> Copy the token)

\- Install SonarCloud as extension from marketplace on Azure DevOps
organization settings. The extension is available in the organization to
add service connection.

-Create new service connection to SonarCloud (Project settings\> Service
connections\>New service connection \> select connection type -
SonarCloud \> Paste the token generated onto SonarCloud token\> give
service connection name\> check grant access permission to all
pipeline\> verify and save )

\- Then you can see these azure pipeline task and create tasks
***prepare analysis configuration***, ***run code analysis***,
***publish quality gate result***

\- Add tasks that prepare analysis configuration(specify the project
key), run code analysis, publish quality gate result in sequence where
we use MSbuild, then run the Azure pipeline

\- After running Azure pipeline, it shows result of code quality
analysis in SonarCloud in different aspects such as reliability,
maintainability, security, issues that concern with the code itself

**Parallel jobs**

\- With Azure DevOps free account, we couldn't even run one pipeline so
that we had to send request to Microsoft to grant to run pipeline job.
Then it allows to run one pipeline job at a time

MS hosted CI/CD - 1 parallel job up to 1800 minutes

Self hosted CI/CD - 1 parallel job

\- For large organizations, they may need to run multiple pipeline jobs
at a time so that you should purchase license for multiple parallel jobs

**Pipeline caching**

\- The pipeline caching basically reduces the build time spends for the
pipeline jobs

\- Some projects may require multiple packages such as NuGet to restore
entire solution, project. These packages should be downloaded on agent
from the internet. This will increase the overall build time for the
pipeline. This where pipeline caching makes the benefit.

\- Hence, it can cache those packages so that they can reuse the
packages for the subsequent pipeline run avoiding download the packages
require for each pipeline run

-In multiple pipeline run, download those packages and add a cache task
to the pipeline

variables:

NUGET_PACKAGES: \$(Pipeline.Workspace)/.nuget/packages

\- task: Cache@2

displayName: Cache

inputs:

key: 'nuget \| "\$(Agent.OS)" \|
\*\*/packages.lock.json,!\*\*/bin/\*\*,!\*\*/obj/\*\*'

restoreKeys: \|

nuget \| "\$(Agent.OS)"

nuget

path: '\$(NUGET_PACKAGES)'

cacheHitVar: 'CACHE_RESTORED'

**Azure pipeline integration with Microsoft Teams**

\- Azure pipeline can be integrated with Teams at specific pipeline as
well as all pipelines in a project. Run these command in Teams after
adding Azure pipeline app into Teams(Microsoft Teams\> Apps\> search the
Azure pipeline \> Add to a team \> set up a bot)

@azure pipeline subscribe \[project URL\] ; you can subscribe all
pipelines as part of the project

@azure pipeline subscribe \[pipeline URL\]

At this stage, you will need to sign into Azure DevOps credentials and
subscribe again

\- Once run Azure pipeline job, the status of the pipeline job is
reflected to MS Teams

**Using GitHub actions**

\- We can create GitHub workflow within GitHub itself to trigger Azure
pipeline in Azure DevOps

To demonstrate GitHub actions,

\- Clone a git repository from GitHub to Visual Studio, open solution
file and create new folder - .github

\- Create a new folder naming workflow within that folder, create a new
item with the template choosing YAML file(workflow.yml)

\- Specify the following in the workflow YAML file

Name of the workflow

Main branch for push - To trigger pipeline from push

Main branch for pull request - To trigger pipeline from pull request

Jobs for the build - ***name*** (Azure pipeline), ***runs-on***( agent
OS), ***azure-devops-project-url***, ***azure-pipeline-name***(you may
use existing pipeline), ***azure-devops-token: \${{
secrets.AZURE_DEVOPS_TOKEN }}*** ( generate PAT from Azure DevOps along
with read and execute permission in build to authorize to work with
pipeline. This token allows to work with the pipeline as part of
project)

name: PipelineWorkflow

on:

push:

branches:

\- main

pull_request:

branches:

\- main

jobs:

build:

name: Azure Pipeline

runs-on: ubuntu-latest

steps:

\- name: Azure Pipelines Action

uses: Azure/pipelines@v1

with:

azure-devops-project-url:
<https://dev.azure.com/techsup4000/AgileProject>

azure-pipeline-name: 'webapp'

azure-devops-token: \${{ secrets.AZURE_DEVOPS_TOKEN }}

\*\* This is a workflow that can run within GitHub repository itself.

\- The publish the git changes to GitHub repository by commit all and
push

\- Generate PAT from Azure DevOps along with read and execute permission
on build for ***secrets.AZURE_DEVOPS_TOKEN***

\- To add secret, select the organization \> Settings \> Security \>
Secrets and variables \> Actions \> Create a New organization secret
specifying the name - AZURE_DEVOPS_TOKEN and value - PAT generated from
Azure DevOps. The PAT works as password that has ability to work with
the builds in Azure DevOps

\- Then as you want, make change on azure DevOps project name by commit
all and push git changes

\- In action pane in GitHub, you can see how workflow change applies
along with detail status of pipeline job. At the same time, you can see
azure pipeline is also in progress

**Jenkins**

**Installing Jenkins**

\- Jenkins is an open source CI/CD tool that the instance should be
hosted on a VM

\- Hosting the Jenkins on Linux VM is viable so that we create Linux VM
in Azure and connect it through putty or VS code

\- Run the following Linux commands to Jenkins installation

sudo apt-get install openjdk-11-jdk-headless ; to install Java
development kit which require to work with Jenkins

wget-q -O <https://pkg.jenkins.io/debian-stable/jenkins.io.key> \| sudo
apt-key add -

sudo ah -c ‘echo deb [http://pkg.debian.io/debian-stable
binary/](http://pkg.debian.io/debian-stable%20binary/) \>
/etc/apt/source.list.d/jenkins.list’

sudo apt update ; update the package index

sudo apt install jenkins ; install Jenkins

sudo ufw allow 8080 ; allow traffic on port 8080 via Linux firewall
rule, Jenkins runs by default on port 8080, this port should be allowed
via NSG as well

sudo systemctl start jenkins; start Jenkins instance

sudo systemctl status jenkins; check status of Jenkins instance

\- Connect to Jenkins instance through
[http://public_IP_of_the_VM:8080](http://public_ip_of_the_vm:8080/)
where to unlock Jenkins and to ensure Jenkins is securely setup by the
administrator, a password must be written to the log file on the
server(/var/lib/jenkins/secrets/initialAdminPassword). The password
should be copied and pasted on to where it should be pasted

sudo -s ; elevate admin privilege to root user

cd /var/lib/jenkins/secrets ; change directory to secret path

more initialAdminPassword ; get the admin password copy and paste on the
web page to unlock Jenkins

\- Customize Jenkins with installing suggested plugins where it starts
to install required plugins

\- After install plugins, it asks to create first admin user with
specifying username and password, full name, email address

-Now you can start using Jenkins

**Jenkins - Creating a build pipeline**

\- Similarly we deploy self-hosted agent with required components, it
needs to install git and .NET SDK on Linux VM that we installed Jenkins
to build the application

sudo apt update ; update package index

sudo apt install git ; install git

git - -version ; check the git version

wget
<https://packages.microsoft.com/config/ubuntu/20.04./packages-microsoft-prod.deb>
-O packages-microsoft-prod.deb

sudo dpkg -i packages-microsoft-prod.deb

rm packages-microsoft-prod.deb

sudo apt-get update;\\

sudo apt-get install -y apt-transport-https && \\

sudo apt-get update && \\

sudo apt-get install -y dotnet-sdk-8.0 ; install .NET SDK on the Linux
VM

We store build and projects in working directory when we create self
hosted agent in Azure DevOps. Similarly we need to give permission this
directory to work with.

sudo chmod -R a+rwx /var/lib/jenkins/

\- Create the build pipeline by creating new item as freestyle project.

Source code management - specify ***git*** and copy/paste ***repository
URL*** from GitHub, add Jenkins credentials to authenticate onto GitHub
account where it username/password of GitHub account, add **\*/main** as
branch to build

Build environment- add build steps for ***execute shell*** “dotnet build
\*.sln” upon any solution file that I have, then save the project

-Select ***Build Now***

\- Once the build is completed, check console output to check the status

**Jenkins Integration with Azure Repos**

\- Create the build pipeline by creating new item as freestyle project.

Source code management - specify ***git*** and ***repository URL*** from
Azure Repos, add Jenkins credentials to authenticate to Azure Repos
where select the ***Clone*** button on the Azure Repos repository and
select ***Generate Git Credentials*** to generate username/password in
order to add into Jenkins credentials, add **\*/main** as branch to
build

Build environment- add build steps for ***execute shell*** “dotnet build
\*.sln” upon any solution file that I have, then save the project

-Select ***Build Now***

\- Once the build is completed, check console output to check the status

\*To trigger the build process in Jenkins automatically how Azure
pipeline does, it needs create service hook in project settings in Azure
DevOps

Service hooks is to integrate with favorite services by notifying when
events happen in project. Then create new service hook subscription with
Jenkins where it installs Azure DevOps Server Plugin on Jenkins to
enhance traceability. Follow below steps for creating service hook in
project settings.

Navigate to project settings \> General \> Service hooks

Service

Select ***Jenkins*** as Select a service to integrate with

Trigger

Trigger on this type of event - Code pushed

Repository - select any repository in the project that the service hook
creates in Azure Repos

Branch - select main or feature branches

Pushed by member of group - select any or specific group in Azure DevOps
project

Action

Perform this action : Trigger generic build

Jenkins base URL :
[http://public_IP_of_the_VM:8080/](http://public_ip_of_the_vm:8080/)

Username: username of Jenkins admin

User API token( or password): go to Jenkins admin and in configure
section, Select ***Add new token*** in API token to generate and copy

Build - select the project created in Jenkins

Once the new service hook subscription is created, you can commit
changes to Azure Repos to trigger the build in Jenkins. Check the
project specified in Jenkins to see the status of continuous integration
cycle

**Managing agents**

\- It is important to consider permission for agent pools. The users
with following roles can manage permission on agent pools.

Reader - can view agent pools and agents

Service account- members in this role can use the organization agent
pool to create a project agent pool in a project

Administrator- in addition to above permission, members of this role can
register or unregister agents from organization agent pool. They can
refer the organization agent pool when create project agent pool

Roles can be managed at the project level

Reader - can view project agent pools

User - use project agent pool when authoring pipeline

Administrator- in addition to above permission, members of this role can
manage membership for all roles of the project agent pool

**Design and implement release pipelines**

**Understand deployment**

\- After building the app using Azure pipeline as part of continuous
integration process, it needs to deploy into Azure VM, Azure Web App or
AKS automatically as users can access the application publicly which is
part of continuous delivery process

\- The process of application deployment goes through following phases.

Test environment - To conduct basic testing to just verify whether it
works properly

Staging environment - To allows set of end users to test the
functionality of the application, basically for UAT

Production environment- Once the end users sign off the acceptance test
by verifying functionalities, publish the application to production
based infrastructure

**Azure Web App - Manual Deployment**

\- Clone a repository from Azure Repos to Visual Studio

\- Create Azure Web App with following specifications.

***Basics***

Subscription, Resource Group

Name of the web app - ***\<name_of_webapp\>.azurewebsites.net***

Publish - code, Docker Container, Static Web App

Runtime stack - .NET 6 or .NET 8

Operating Systems- Linux, Windows

Region

Under App Service Plan, SKU and size -(Dev/Test, Production, Isolated)
and (Basic, Standard)

***Deployment***

GitHub Actions settings - Enable/disable Continuous deployment

GitHub Actions details - GitHub account

***Networking***

Enable network injection - on/off

***Monitoring***

Disable Application insight

\- Publish the app from VS to Azure creating publish profiles as
*target* specifying Azure app service as *specific target*,
subscription/Resource group/choose app service instance as App service,
Publish(generates pubxml file) as deployment type, then publish

\- Visual Studio first build the application and create publish version
of the application, the copy it onto Azure App service

**Azure Web App - Release pipeline**

\- Ensure Azure build pipeline runs properly with basics that includes
trigger, pool, NuGet package installer, build and publish tasks

\- Turn off “Disable creation of classic release pipeline “ in pipeline
at Organization settings

\- You have YAML format and classic version when you create release
pipeline

\- On template offering, create empty job with appropriate naming for
new stage that allow to define environments such as test, staging and
production

Artifacts is what we want to deploy where it is the build of the
application.

Add an artifact -Source type(Where the build pipeline remains), Project,
Source(build pipeline), Default version

\- Once the build pipeline is triggered, it will create a build and the
build will be transferred as an artifact onto entire release pipeline.

\- Create an agent job in deployment stage where release of the
application also require an agent to run command to release the
application. This is an agent pool that ***Hosted Windows 2019 with
VS2019*** agent

\- In the agent job, you can define ***Azure Web App Deploy*** task
along with Azure subscription(login to Azure portal to authorize which
create service connection internally from Azure DevOps to Azure
subscription), App type( Web App on Windows, Web app on Linux), App
name( the Azure web app that already created) for a task. Then provide a
name for the release pipeline

\- Create release with the artifact and stages added. Once you click the
release created, it starts release pipeline to be triggered and to
install the build onto target environment

\- If job fails, you can check logs for more understanding. Even though,
the build is sourced from a build pipeline, the build will not be
available as it uses Microsoft hosted agent for the build

\- Hence, the build of the application must be transferred from build
environment to release environment, you should add
***PublishPipelineArtifact*** task into build pipeline

\- task: DotNetCoreCLI@2

inputs:

command: publish

publishWebProjects: True

arguments: '--configuration \$(BuildConfiguration) --output
\$(Build.ArtifactStagingDirectory)'

zipAfterPublish: True

\# We still need to take the staging directory files and publish it as a
build artifact

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.ArtifactStagingDirectory)'

artifactName: 'webapp-artifact' ; name of the artifact we create in
release pipeline

\- The publish pipeline artifact publishes artifact from build artifact
staging directory into the build pipeline even after the Microsoft
hosted agent is destroyed after the build is made

\- Enable continuous deployment trigger before you trigger build
pipeline. Thereby any change makes to build pipeline triggers the
release pipeline automatically.

**Multiple stages in the pipeline**

\- We can maintain test and staging environments to check new build is
working properly prior to release onto production environment

\- Add new empty stage for staging environment with task - Azure Web App
Deploy specifying target environment

\- The make change on project in Azure Repos which start to trigger
build and release pipeline and to deploy on test and staging environment
stages

**Approvals and gates**

\- When release pipeline is complete to test environment, users should
have certain time to go through testing scenarios. Once testing
complete, the release can be deployed to staging environment

\- Hence ***approvals*** and ***gates*** are used to manage transition
between stages

Pre-deployment approval- A user needs to validate the change request so
that the deployment can be done to that stage

Post-deployment approval- An user needs to sign off on the deployment
done so that it can move to another stage

Approvals are manual approaches whereas gates are automate approaches

\- Assume that there work items in Azure boards that are active and the
build deploys on test environment have bugs identified which are also
registered on Azure boards. Before the build can go to next stage, you
have to ensure all the bugs and work items in Azure Boards are closed.

Pre-deployment gate - An user wants to ensure that no work items are
active for the build to be deployed to a stage

Post-deployment gate - A user wants to ensure that no issues or bugs are
tagged against a deployment before it can proceed to the next stage

**Release pipeline - Approvals**

\- Pre-deployment approvals can be enabled with defining timeout value
where deployment will not carry out to stages if approvers won’t approve
with timeout period

\- After committing a change on the project, build pipeline complete.
The release pipeline start to trigger once approver provide approval
from email or Azure DevOps portal

**Azure pipeline- Gates - Query work items**

\- If you enable gates, first it needs to disable pre-deployment
approvals

\- Create shared query on Azure Boards to filter out work items that
that are not closed(operator is \<\>)

\- Add post-deployment gate adding query work items with shared query we
have created where it has evaluation option as well, the delay time
before evaluation

***Deployment gate types***

1.  Check Azure policy compliance

2.  Invoke Azure Function

3.  Invoke REST API

4.  Query Azure Monitor alerts

5.  Query work items

6.  SonarCloud Quality Gate status check

\- Before release pipeline to proceed, allow read permission for user
for particular project build service on shared queries

\- Then create release which start to run along with post deployment
gate condition. If the post-deployment condition fails, it continues
re-evaluation with defined time period until deployment condition fails
or passes

**Azure pipeline- Gates- Azure Monitor alerts**

\- We can define post-deployment conditions for Azure monitor alerts
based on activity logs, metrics, logs and service health

\- For instance, create alert rule with condition of average memory of
Azure web app and define post deployment gate with query Azure Monitor
alerts where we can specify filter type, alert rule created time range,
alert state, monitor condition.

\- Azure Monitor alerts should be cleared in order to release pipeline
to be proceeded from one stage to another

**Azure pipeline- Gates- Azure policies**

\- We can define post-deployment conditions for compliance status of
Azure policy

\- For instance, create Azure policy definition and assignment for not
allowed resource types for a resource group and also create not allowed
resource in resource group, then create post deployment gate with check
Azure policy compliance

\- Azure policy needs to be compliant in order to release pipeline pass
the gate from one stage to another

**Azure release - Manual Intervention**

\- This involves agentless job with a task - manual intervention before
it goes to agent job in the stages

\- The manual intervention task includes to add instruction to notify an
user whether agentless job can be resumed or rejected in the stage
manually

\- It needs to disable existing pre and post deployment approvals and
gates on stages prior to add agentless job

**Deployment Groups - Setup & Implementation**

\- Some application needs to deploy to multiple machines at a time

\- You can place them as part of a deployment group

\- An agent needs to be installed on each machine

\- Create multiple Azure VMs, then install IIS and ASP.NET Core 6 on
VMs, further allow port 80 inbound on NSG

\- To implement deployment group, it needs to create deployment group
which provide registration script based on target either Windows or
Linux.(Azure DevOps \> Pipeline \> Deployment group)

\- Select to ***use personal access token in the script for
authentication*** before copy the script

\- Copy the registration script and run on Windows PowerShell at target
VMs

<img src="./images/1b0090bd71ce800c1963c0c31f6520123ee3906c.png"
style="width:7.47917in;height:3.16667in" />

\- Through the script, the VM connect to Azure DevOps server and scan
tool capabilities, enter deployment group tags for agent(default No),
Enable SERVICE_SID_TYPE_UNRESTICTED for agent service(default No), User
account to use for the service(default value), enter default values that
the script offer

\- Once the target VMs are registered with the deployment group, they
shows as targets

\- You can add new stage to proceed build and release pipeline on to
deployment group job

\- Remove if there is an agent job and add a deployment group job
instead where you should specify the deployment group, targets to deploy
to in parallel(multiple/one target at a time), Artifact download

\- Additionally add ***IIS web app manage*** task where we specify
Display name, Configuration type- IIS Website, Action - Create or
Update, Web site name, Physical path

-Add ***IIS web app deploy*** task, where we specify Display name, Web
site name and save the new stage

\- Once create release, it triggers and deploy artifacts on targets VMs
in deployment group. These VMs might be Azure VMs or on-premise VMs

**Azure Web App - Azure SQL database**

\- Deploy Azure SQL database for .NET core web app to connect

\- Create a ***SQL database*** specifying database name, server
name(***\<server_name\>.database.windows.net***, location),
Authentication method(SQL authentication, admin login with password),
workload environment, configure database, service tier, connectivity
method- public endpoint, Firewall rules -allow Azure service and
resources to access this server and add current IP address.

\- Connect SQL database with admin user credentials using query editor
and run query to create a table with column and values

\- Connecting SQL database and running SQL script can be performed as
part of release pipeline as well

-Open the project from VS and navigate to service folder, open
***Service/ProductService.cs*** file in the project and navigate to
ProductService public class

-Specify database server, username, password and database in the
***productservice.cs*** file, run the app on VS locally which fetch the
data from Azure SQL database and show the table outputs on browser
locally

**Deploying Azure Web App**

\- Create Azure Web app with runtime stack and publish. It create naming
***\<webappname\>.azurewebsites.net***

\- Create git repository on Azure Repos and push the project from Visual
Studio

\- Set up build from the project along with vmImage, NuGet tool
installer, NuGet command, DotNetCoreCLI for build, DotNetCoreCLI for
publish and PublishPipelineArtifact tasks. These are the components
basically in build pipeline.

\- Create a release pipeline with build artifact where enable continuous
deployment trigger and a stage that includes agent job with ***Azure Web
app*** task

\- The run the build pipeline which start to trigger build and release
pipeline, end up with deployment to Azure Web App

-The output for Azure web app is database table where the project code
deployed to Azure web app connects through static string from published
code itself to Azure SQL database

**Azure pipeline - SQL Database table**

\- We can deploy database table into Azure SQL database using release
pipeline so that add the task Azure SQL Database deployment into agent
job in release pipeline

\- Create ***Azure SQL Database deployment*** task to create a table and
insert data into the table. In that task, specify display name, Azure
connection type, Azure Subscription, Authentication type- SQL server
authentication, Azure SQL server, database, login credentials to
DB(username, password), Deploy type- Inline SQL script, insert the
inline SQL script for table creation

\- Create ***Azure Web App*** task to pick up web application and deploy
onto Azure Web App

**Azure pipeline - Azure Web App - Connection String**

\- It is a bad practice hardcoding SQL server name, DB username and
password, SQL database into the source code project using static string

\- Instead you can create connection string in configuration settings in
Azure Web App in order to connect to Azure SQL database from Azure Web
App. Add name, type - SQLAzure, value- copy database connection strings
from overview page in Azure SQL database - ADO.NET(SQL authentication)
where we need to specify the password of DB in that ADO.NET value.
However, this is the manual approach to use connection string in Azure
Web App

\- In the source code project, you should specify
*connection_string_name* in SqlConnection GetConnection() private class
to fetch connection string details using ***GetConnectionString*** from
Azure Web App in order to connect with database

\- We can add connection string into Azure Web App in automated way by
adding Azure App Service Settings task into job in release pipeline. In
the task, you should place subscription, App service name, resource
group, connection string along with the password

\- Since we make source code with *connection_string_name* reference, we
should publish the code by creating git repository into Azure Repos and
create new build pipeline with artifact

-Additionally to above release, create ***Azure App Service Settings***
task in the release pipeline after ***Azure Web app*** task by selecting
Azure Subscription, App Service name, resource group and Connection
Strings(name: c*onnection_string_name,* value - copy database connection
strings from overview page in Azure SQL database - ADO.NET(SQL
authentication) where specify the password of DB in the value)

\- There may be error as the SQL table has values when run task in
release pipeline. In that case, change SQL script in the task to check
availability of values first before adding values into the table. (Check
the reference)

-Then trigger the release pipeline

**Release pipeline- Associate work items**

\- Release pipeline can be integrated to report deployment status to
work stages so that edit release and go integration in options

\- Then commit a change into Azure Repos git repository by linking a
work items using ***Works items to link*** in commit page

\- After completing build and release pipeline, the status of deployment
shows on link section on work item as commit number along with commit
message and integrated in release stage \<name of release pipeline\>and
state

**Containers**

\- We have deployed .NET Core application into Azure Web App and virtual
machine

\- For containerized application deployment, we need to go through these
steps

1\. Install Docker on a VM

2\. Publish the build of .NET application onto the VM that Docker
installed

3\. Create docker custom image using Dockerfile

4\. Publish the custom image to private registry in Azure Container
Registry(ACR)

5\. Use that image to deploy the container either Azure Container
Instance(ACI) or Azure Kubernetes services(AKS)

**Building a Docker image - Manual approach**

\- Hard code SQL server name, username, password and SQL database on
product service file in the project(Or else we can specify Azure SQL
database credentials using connection string on ***GetConnection***
private class)

\- Create a Ubuntu VM with docker engine installed and connect the VM
with putty

\- Refer the necessary Docker documentation to install docker engine on
the Ubuntu VM

\- Publish the project that build onto directory in local directory by
creating publish profile

\- Copy the published build into Ubuntu VM using WinSCP tool where you
need to connect to the VM over public IP over WinSCP

\- Create ***Dockerfile*** to make docker image

FROM mcr.microsoft.com/dotnet/aspnet:6.0 ; get base image that container
ASP.NET 6.0 runtime

WORKDIR /app ; create a working directory

COPY . . ; copy the build files into image

EXPOSE 80 ; exposing the application from port 80

ENTRYPOINT \[“dotnet”, “sqlapp.dll”\] ; run application file that run
within the container

\- Copy the Dockerfile into the directory where the sqlapp.dll is placed
on Linux VM via WinSCP

\- Go the directory on Linux VM where the Dockerfile is placed in

\- Run the following command to build custom docker image

***sudo docker build -t sqlapp . ;*** build container image with sqlapp
tag

***sudo docker images*** ; list the docker images with image ID

**Deploying a container - Manual approach**

\- Create a container registry on Azure to publish docker image built on
to container registry . Provide registry
name(***\<registryname\>.azurecr.io***)

\- Install Azure CLI tool on Linux VM(Refer Microsoft Documentation)

\- Log into Azure container registry. To get access credentials, open
access keys in ACR and enable admin user where you can see username and
passwords, copy them into clipboard

sudo az acr login - -name \<container registry name\> - -username
\<username\> - -password \<password\>

\- Tag the docker image you built

sudo docker tag \<docker image name\>
\<containerregistryname\>.azurecr.io/\<ACR image repository name\>

\- Then push the image to the Azure Container Registry. Once push is
complete, the container image is available in the repository section in
ACR

sudo docker push \<containerregistryname\>.azurecr.io/\<ACR repository
name\> ;

\- Create Azure Container Instance to spin up a container based on
container image. Specify container name, image source(QuickStart
images/Azure container registry/other registry) for ACR it picks up
registry, image, image tag and OS type- Linux, size- Change size of
compute as you want, Networking type- public with TCP port 80

\- From the public IP of ACI, you can access the SQL application
running, since SQL database is open to internet, the container can
interact with SQL database because the project code has hardcoded
credentials to connect with SQL database.

**Azure pipeline - Azure container registry**

This is automated method to deploy containerized application into ACI.

\- Create source code of project and Dockerfile and copy the Dockerfile
into project folder.

\- Create git repository for the project on Azure Repos and push it from
Visual Studio

\- Set up build pipeline from Azure Repos where it shows Docker option
***Build and push an image to ACR*** as Azure DevOps identifies that the
Azure Repos includes Dockerfile. Once choose Docker option, it starts
wizard to create service connection to ACR from Azure DevOps by logging
in to Azure subscription

\- Provide Azure credentials to authorize with service connection to ACR
where specify container registry name, image name, Dockerfile-
\$(Build.SourcesDirectory)/\<projectname\>/Dockerfile(it automatically
gets the Dockerfile as it includes in the project folder from prebuild
variable that is source directory), then validate and configure

Note: If you don’t see container registry name, you should relogin in to
Azure DevOps to make sure service connection is established with ACR
properly

Docker YAML file includes,

1\. Trigger is same to build the code

2\. Resources is self where it takes the Dockerfile from repository that
YAML file is referring to

3\. In variables, Container registry service connection established
during pipeline creation which have service connection -
***dockerRegistryServiceConnection***, image repository name
***imageRepository***, container registry name, dockerfilePath, tag,
vmImageName is 'ubuntu latest'

4\. In stages, there are stages for build and Push the image

5\. In steps, there is a Docker task ***buildAndPush*** the image to ACR

\*\*Thus, the image build is created wrongly. We consider correct way to
build the image

\- There are few differences between .NET and Docker YAML files for
build pipeline. In this pipeline, it gets source code directly from the
repository instead of the build of the source code. Hence, we should add
steps to build from the source code, then take built code to create an
image

\- Add task installing .NET SDK doing build of the project and doing the
publish before the Docker task ***buildAndPush***

\- Add ***buildContext*** into Docker task to get from
***\$(BuildArtifactStagingDirectory)*** with required tagging, save the
pipeline and run

\- Go to ACR, check the containerized image pushed in the repository

\- Create Azure container instance with the image from ACR and open TCP
port 80 publicly from networking

-After ACI is created, container is being run and access the application
from public IP address of ACI

trigger:

\- main

resources:

\- repo: self

variables:

\# Container registry service connection established during pipeline
creation

dockerRegistryServiceConnection: 'b3020420-c1f5-447c-acb1-0da44fc27f2c'

imageRepository: 'sqlappdocker'

containerRegistry: 'localregistry1000.azurecr.io'

dockerfilePath: '\$(Build.SourcesDirectory)/sqlapp/Dockerfile'

tag: '\$(Build.BuildId)'

\# Agent VM image name

vmImageName: 'ubuntu-latest'

stages:

\- stage: Build

displayName: Build and push stage

jobs:

\- job: Build

displayName: Build

pool:

vmImage: \$(vmImageName)

steps:

\- task: UseDotNet@2

inputs:

packageType: 'sdk'

version: '6.x'

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: DotNetCoreCLI@2

inputs:

command: publish

publishWebProjects: True

zipAfterPublish: false

arguments: '--configuration \$(BuildConfiguration) --output
\$(Build.ArtifactStagingDirectory)'

\- task: Docker@2

displayName: Build and push an image to container registry

inputs:

command: buildAndPush

buildContext: '\$(Build.ArtifactStagingDirectory)/sqlapp'

repository: \$(imageRepository)

dockerfile: \$(dockerfilePath)

containerRegistry: \$(dockerRegistryServiceConnection)

tags: \|

\$(tag)

latest

**Azure pipelines - Azure Container Registry- Debugging**

-The Docker task may still take the source code instead of the build in
artifact staging directory

\- To list and verify the files in Build.ArtifactStagingDirectory are
built properly, add PowerShell task after .NET Core publish task into
YAML file for build pipeline which shows files with size, name,
permission level in path '\$(Build.ArtifactStagingDirectory)/sqlapp'
that gets to build container image

\- pwsh: \|

Get-ChildItem -Path \$(Build.ArtifactStagingDirectory)\\.\* -Recurse
-Force \| Out-String -Width 180

errorActionPreference: continue

displayName: 'List content'

continueOnError: true

**Azure Container Instance - Release pipeline**

\- We create new release pipeline to deploy container image in azure
container registry into Azure Container Instance. We don't need artifact
in the release pipeline

\- Add new stage as deployment to container, which create agent job with
Microsoft hosted agent. Add task ***Azure CLI*** task to interact with
Azure resource(use Azure PowerShell alternatively)

\- Select Azure Resource Manager connection- Azure Subscription, script
type- Batch, script location- Inline script, write the script as follows

az container create -g devops-grp - -name \<container instance name\> -
-cpu 1 - -memory 1 - -ports 80 - -ip-address \<Public IP address name\>-
-image registry566.azurecr.io/sqlappdocer:latest - -registry-username
\<username\> - -registry-password \<password\>

Note: Specify the public IP address in the command. If you don't mention
it, the IP address would be private IP address.

\- In the release pipeline, we don’t specify container image pushed
already onto ACR and also we manually run the release pipeline

**Deployment to Azure Kubernetes Service - Manual approach**

\- Create Azure Kubernetes Service with following config settings.

Basics- cluster preset configuration(Production Standard, Dev/Test,
Production Economy, Production Enterprise), Kubernetes cluster name,
region, availability zone(no), AKS pricing tier(Free, Standard,
Premium), Automatic upgrade(cluster upgrade based on new AKS and
Kubernetes releases), Node security channel type (for node level
security updates), Authentication and authorization(native Kubernetes
RBAC, Azure RBAC)

Node pool - Node pool name, Mode(system, user), OS SKU(Azure Linux,
Ubuntu Linux, Windows), availability zone,

, Enable Azure Spot instances, Node size, Scale method(Manual,
Autoscale), Minimum node count, Maximum node count, Max pods per node,
Enable public IP per node, Labels(Key, Value), Taints(Key, Value,
Effect)

Networking

Integration - Specify Azure container registry

\- Create deployment manifest file and service manifest file with
container image pushed to ACR

Deployment manifest file - create containers by specifying container
image from ACR along with replicas

Service manifest file - Load balancer type service to expose the
containers to external

\- Navigate workload in Kubernetes resources and create with YAML file,
copy the content of deployment, add

\- Navigate Services and ingresses in Kubernetes resources and create
with YAML file, copy the content of service manifest file, add

\- Once workloads create, the deployment will be ready state after
certain time

\- The LoadBalancer service type will be OK with External IP, the app is
accessible from public IP

**YAML Pipelines - Deployment to Azure Kubernetes Service**

\- The build pipeline we created to build the container image and
publish onto Azure container registry can use to extend in order to
deploy image onto Azure Kubernetes service

\- In project settings, first we need to create service connection to
Kubernetes cluster by specifying service connection name

\- Choose authentication method- Azure subscription(provide
credentials), select the AKS cluster, namespace(default), give name for
service connection, then save

\- Add deployment and service manifest files into a folder in the source
code project in VS by creating new folder and adding manifest files into
the folder, commit all and push the changes into Azure Repos(Stop the
trigger of build pipeline if it automatically triggers)

\- Add ***Deploy to Kubernetes*** task into build pipeline after docker
task as following details. Please make sure to have right indentation
and commit the change.

Action- deploy

Kubernetes service connection- the service connection

Manifests- app.yml

Add the path of manifest files by removing app.yml as above.

\$(Build.SourcesDirectory)/sqlapp/Manifests/app.yml \>\> for deployment

\$(Build.SourcesDirectory)/sqlapp/Manifests/service.yml \>\> for service

\- The deployment will be ready state after certain time

\- The LoadBalancer service type will be OK with External IP, the app is
accessible from public IP

\- task: KubernetesManifest@0

inputs:

action: 'deploy'

kubernetesServiceConnection: 'kubernetes-connection'

manifests: \|

\$(Build.SourcesDirectory)/sqlapp/Manifests/app.yml

\$(Build.SourcesDirectory)/sqlapp/Manifests/service.yml

**Release pipeline- Azure Kubernetes Service**

\- Previously we have done the deployment using build pipeline, now we
do it using release pipeline

\- Remove deploy to Kubernetes task from build pipeline instead add
***PublishPipelineArtifact*** task to publish all source code files to
release pipeline and commit changes

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Pipeline.Workspace)'

artifact: 'sourcefiles'

publishLocation: 'pipeline'

\- This task will publish artifacts as part of build pipeline

\- Create new release pipeline, add an artifact by selecting project and
you can find the published artifact in 'sourcefiles' and manifests files
I Manifest in **s** directory

\- Create new agent job and add separate tasks for Manifest files using
***Deploy to Kubernetes*** task

\- Name those tasks as *app.yml deployment* and *service.yml
deployment,* action- deploy, kubernetes Service Connection, create a
release to trigger the pipeline

\- The deployment will be ready state after certain time

\- The LoadBalancer service type will be OK with External IP, the app is
accessible from public IP

**Publish artifacts**

\- The YAML pipeline ***azure-piplines.yml*** you create is part of your
code repository. So the YAML file is also versioning with each commit
when you check the history

\- Using ***PublishPipelineArrifact*** task, we publish all source files
from build to release pipeline. Instead we can publish files selectively
on to release pipeline

**Multi-stage builds**

\- The purpose of mutli-stage build is to perform build and publish with
the help of Dockerfile

-Store the Dockerfile as part of the source code

FROM MCR.microsoft.com/dotnet/sdk:6.0 AS build

WORKDIR /source

COPY \*.csproj ./

RUN dotnet restore

COPY . .

RUN dotnet publish -c Release -o out

FROM mcr.microsoft.com/dotenet/aspnet:6.0

WORKDIR /app

COPY - -from=build /source/out .

EXPOSE 80

ENTRYPOINT \[“dotnet”, “sqlapp.dll”\]

\- Save the Dockerfile, commit all and push changes

\- If there are changes on git repository on Azure Repos, it pull and
push from repository

\- As we do build and publish using Dockerfile, we can delete install
.NET SDK task and .NET Core task for build and publish tasks from build
pipeline and remove **buildcontext** for
***BuildArtifactStagingDirectory*** from Docker task because we don’t
need to specify artifact directory, save the build pipeline

trigger:

\- main

resources:

\- repo: self

variables:

\# Container registry service connection established during pipeline
creation

dockerRegistryServiceConnection: 'b3020420-c1f5-447c-acb1-0da44fc27f2c'

imageRepository: 'sqlappdocker'

containerRegistry: 'localregistry1000.azurecr.io'

dockerfilePath: '\$(Build.SourcesDirectory)/sqlapp/Dockerfile'

tag: '\$(Build.BuildId)'

\# Agent VM image name

vmImageName: 'ubuntu-latest'

stages:

\- stage: Build

displayName: Build and push stage

jobs:

\- job: Build

displayName: Build

pool:

vmImage: \$(vmImageName)

steps:

\- task: Docker@2

displayName: Build and push an image to container registry

inputs:

command: buildAndPush

buildContext: '\$(Build.ArtifactStagingDirectory)/sqlapp'

repository: \$(imageRepository)

dockerfile: \$(dockerfilePath)

containerRegistry: \$(dockerRegistryServiceConnection)

tags: \|

\$(tag)

latest

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Pipeline.Workspace)'

artifact: 'sourcefiles'

publishLocation: 'pipeline'

**Container jobs**

\- The compute instance in this case is Microsoft-hosted agent. The
build run on a compute instance. The Microsoft-hosted agent is one time
resource unlike self-hosted agent

\- A self-hosted agent can use repeatedly for multiple builds. However,
it needs different tools and packages to be installed for when it uses
for multiple application to make build which may happen conflict with
different packages

\- The agent has certain capabilities

\- As solution for this case Azure DevOps provides use of container job
where containers have their own tools required for the build to run.
This way, we can save the cost significantly

**Working with container job**

\- We have multiple stages in YAML file in build pipeline for build and
deploy where we don’t have task for installing .NET SDK because build
and publish tasks are running on a container

-All the tasks under the job are running on container with base image
specified

trigger:

\- main

resources:

\- repo: self

variables:

\# Container registry service connection established during pipeline
creation

dockerRegistryServiceConnection: 'b3020420-c1f5-447c-acb1-0da44fc27f2c'

imageRepository: 'sqlappdocker'

containerRegistry: 'localregistry1000.azurecr.io'

dockerfilePath: '\$(Build.SourcesDirectory)/sqlapp/Dockerfile'

tag: '\$(Build.BuildId)'

\# Agent VM image name

vmImageName: 'ubuntu-latest'

stages:

\- stage: Build

displayName: Build stage

jobs:

\- job: Build

displayName: Build

pool:

vmImage: \$(vmImageName)

container: mcr.microsoft.com/dotnet/sdk:6.0 ; base image use for the
container

steps:

\- task: DotNetCoreCLI@2

inputs:

command: build

projects: ‘\*\*/\*.csproj’

arguments: ‘- -configuration \$(buildConfiguration)

\- task: DotNetCoreCLI@2

inputs:

command: publish

publishWebProjects: True

zipAfterPublish: false

arguments: ‘- -configuration \$(buildConfiguration) - -output \$(
Build.ArtifactStagingDirectory)’

\- publish: ‘\$( Build.ArtifactStagingDirectory)’

displayName: ‘Publish build’

artifact: buildartifacts ; publish the artifact to release pipeline

\- stage: Deploy

displayName: Push stage

jobs:

\- job: Deploy

displayName: Deploy

pool:

vmImage: \$(vmImageName) ; this job is running in the VM, not in the
container

steps:

\- download: current

artifact: buildartifacts ; download the build artifact created into
release pipeline

\- task: Docker@2

displayName: Build and push an image to container registry

inputs:

command: buildAndPush

buildContext: ‘\$(Pipeline.Workspace)/buildartifacts/sqlapp’

repository: \$(imageRepository)

dockerfile: \$(dockerfilepath)

containerRegistry: \$(dockerRegistryServiceConnection)

tags:

\$(tag)

latest

\- With download steps, the build artifact will be downloaded onto
deploy agent job

\- From the basic Dockerfile, build container image and push to ACR

-After this task you can deploy the container image to ACI or you can
deploy the build on to AKS cluster by adding the task - ***Deploy to
Kubernetes*** (KubernetesManifest@0) into YAML pipeline with build and
push stages.

\- task: KubernetesManifest@0

inputs:

action: ‘deploy’

kubernetesServiceConnection: ‘Kubernetes-connection’

manifests: \|

\$(Build.SourcesDirectory)/sqlapp/Manifests/app.yml

\$(Build.SourcesDirectory)/sqlapp/Manifests/service.yml

\- Save this pipeline and commit the changes to trigger the pipeline

**Technical Debt**

\- Sonarcloud helps to maintain the stability and quality of the
application code over the time with the maintainability

SonarQube is a set of static analyzers that can be used to identify
areas of improvement in your code. It allows you to analyze the
technical debt in your project and keep track of it in the future. With
Maven and Gradle build tasks, you can run SonarQube analysis with
minimal setup in a new or existing Azure DevOps Services build task.
Prepare Analysis Configuration task, to configure all the required
settings before executing the build. ✑ This task is mandatory.✑ In case
of .NET solutions or Java projects, it helps to integrate seamlessly
with MSBuild, Maven and Gradle tasks.

The percentage of overall time spent on rework-Technical Debt is the
estimated cost to fix code elements issues.

Technical Debt Ratio: Ratio between the cost to develop the software and
the cost to fix it. The Technical Debt Ratio formula is:

Remediation cost / Development cost

Which can be restated as: Remediation cost / (Cost to develop 1 line of
code \* Number of lines of code)

The lead developer at your company reports that adding new application
features takes longer than expected due to a large accumulated technical
debt. You need to recommend changes to reduce the accumulated technical
debt: reducing code coupling and dependency cycles can be an effective
way to reduce accumulated technical debt. Technical debt can occur when
developers take shortcuts, such as copying and pasting code or creating
dependencies between different parts of the codebase. This can lead to
an accumulation of technical debt over time, which makes it harder to
add new features or make changes to the existing codebase. Reducing code
coupling and dependency cycles can help break down these dependencies
and make the codebase more modular and easier to work with. By reducing
code coupling, you can make it easier to modify specific parts of the
codebase without affecting other parts. Similarly, by reducing
dependency cycles, you can break down complex relationships between
different parts of the codebase and make it easier to understand and
modify the code

Reduce the code complexity. Note: Technical debt is the accumulation of
sub-optimal technical decisions made over the lifetime of an
application. Eventually, it gets harder and harder to change things:
it's the 'sand in the gears' that sees IT initiatives grind to a halt.
Reusability measures whether existing assets—such as code—can be used
again. Assets are more easily reused if they have modularity or loose
coupling characteristics. The number of interdependencies can measure
reusability. Running a static analyzer can help you identify these
interdependencies

**When there are multiple builds**

\- When you have multiple builds coming on to release pipeline at same
time, you can decide what is the maximum number of parallel deployment
you want to have in place using ***deployment queue settings*** in the
pre-deployment conditions to consider.

\- It has following options

Number of parallel deployments - Specific/Unlimited

Deploy all in sequence

Deploy latest and cancel the others- discard the old builds and deploy
the latest build

**Design and Implement Infrastructure as Code**

**Managing infrastructure**

\- Creating your infrastructure can be done using release pipeline

\- Making changes on infrastructure based on the resource consumption
such as increasing VM size

\- Some organization maintains multiple environments with identical
infrastructure for application deployment such as development, test,
staging and production. Replicating the same infrastructure across
multiple environments is required

\- Sometimes you might not document properly how you built your
infrastructure at first place

\- To simplify and accomplish above all, you develop your infrastructure
as code

\- This helps clearly define how you infrastructure should look like

\- You can easily make changes to your infrastructure with the help of
changes to the code file

\- You can also version control the code file that is used to define
your infrastructure

\- Replicating your infrastructure across multiple environments

\- ARM templates, Bicep are popular Azure tool for IaC, while Terraform
is the industry leader in IaC

\- Azure CLI and Azure PowerShell modules are used to deploy and manage
resources using scripts

**ARM Template**

\- In this case, we deploy Azure web app for web server and Azure SQL
database for database server

\- Create an Azure Resource Manager template for defining infrastructure
as code

\- This is a JSON file that actually contains the definition of the
infrastructure

\- You can store the ARM templates in your source code repository along
with your application code

\- Microsoft has also released a new language called Bicep that has the
same capabilities as ARM templates

\- Bicep just uses a syntax that is easier to use.

\- Parameters uses to send values dynamically to template

\- Install Azure Resource Manager(ARM) tools extension on VS code which
allows you to quickly create ARM template VS code

{

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"languageVersion": "",

"contentVersion": "",

"apiProfile": "",

"definitions": { },

"parameters": { }, ; to dynamically send values to the template

"variables": { },

"functions": \[ \],

"resources": \[ \], /\* or "resources": { } with languageVersion 2.0 \*/
; for resources we create

"outputs": { }

}

**ARM Template- Azure Web App**

\- To deploy Azure Web App, Azure web app and app service plan should be
in place

\- With apiVersion you select, there might be slight change when it
comes resource format

\- Use in built function to define location of resource to get it from
location of resource group

\- App service plan gets resources type as
***Microsoft.Web/serverfarms***. Define name,
location(\[resourceGroup().location\]), SKU, capacity

\- Azure web app gets resources type as ***Microsoft.Web/sites***.
Define ***serverFarmId*** using ***resourceId*** function adding
resource type and resource name of app service plan to link Azure web
app with App service plan

\- Add ***dependson*** clause to specify dependency of app service plan
with Azure web app so that add the ***resourceId*** created with

\- You can deploy ARM template using PowerShell, VS code or template
deployment in Azure

\- Create a resource group and copy ARM template code onto template
deployment, create

{

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"contentVersion": "1.0.0.0",

"parameters": {},

"functions": \[\],

"variables": {},

"resources": \[

{

"type": "Microsoft.Web/serverfarms",

"apiVersion": "2022-03-01",

"name": "plan787878",

"location": "\[resourceGroup().location\]",

"sku": {

"name":"F1",

"capacity":1

},

"properties":{

"name":"plan787878"

}

},

{

"type": "Microsoft.Web/sites",

"apiVersion": "2022-03-01",

"name": "newapp994848",

"location": "\[resourceGroup().location\]",

"properties":{

"name":"newapp994848",

"serverFarmId":"\[resourceId('Microsoft.Web/serverfarms','plan787878')\]"

},

"dependsOn":\[

"\[resourceId('Microsoft.Web/serverfarms','plan787878')\]"

\]

}

\],

"outputs": {}

}

**ARM Templates- Azure SQL database**

\- To deploy Azure SQL database, server to host the database and
database itself should be in place

\- Provider of SQL server define as ***Microsoft.SQL/servers*** which
needs admin login and password specify via parameters of the template.
Define parameter type for SQLLogin as string and SQLPassword as
secureString, further name, location, properties(refer properties from
parameters)

\- Provider of SQL database define as ***Microsoft.Sql
servers/databases*** which SKU name and tier to specify.

\- Add ***dependson*** attribute to specify dependency of database
server with database so that add the ***resourceId*** created with

\- Name the database with format function along with database server

\- You can deploy ARM template using template deployment in Azure

\- Create a resource group and copy ARM template code onto template
deployment in Azure by inserting ***SQL login*** and ***SQL password***
which create the database with master database on SQL server, create

{

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"contentVersion": "1.0.0.0",

"parameters": {

"SQLLogin": {

"type":"string",

"metadata":{

"description":"The administrator user name"

}

},

"SQLPassword": {

"type":"secureString",

"metadata":{

"description":"The administrator password"

}

}

},

"functions": \[\],

"variables": {},

"resources": \[

{

"type": "Microsoft.Sql/servers",

"apiVersion": "2022-02-01-preview",

"name": "sqlserver400505",

"location": "\[resourceGroup().location\]",

"properties":{

"administratorLogin": "\[parameters('SQLLogin')\]",

"administratorLoginPassword": "\[parameters('SQLPassword')\]"

}

},

{

"type": "Microsoft.Sql/servers/databases",

"apiVersion": "2022-02-01-preview",

"name": "\[format('{0}/{1}','sqlserver400505','appdb')\]",

"location": "\[resourceGroup().location\]",

"sku":{

"name":"Basic",

"tier":"Basic"

},

"properties":{},

"dependsOn":\[

"\[resourceId('Microsoft.Sql/servers','sqlserver400505')\]"

\]

}

\],

"outputs": {}

}

**ARM Template - Azure virtual machine**

\- When create Azure VM, the following dependent resources should be
created.

Virtual network - host the network

Subnet- sub network in the network created

Network interface - to assign private or public IP address on to VM

Public IP Address - to access the VM from the Internet

Data disk - for data disk on the VM if needed

Network Security Group - to restrict the VM with inbound and outbound
traffic

Storage account - to store boot diagnostics of the VM

\- Structure the ARM template with creating above resources

\- Create virtual network adding address prefix into properties section

\- Add subnet address prefix into properties section and define id using
***resourceId*** function adding resource type and resource name of NSG
to link subnet with NSG

\- Create another subnet with no link to NSG

\- Create public IP address with properties
***publicIPAllocationMethod*** as Dynamic

\- Create network interface with properties ip configurations, then link
network interface with PIP and subnet with ***resourceId*** function.
Add dependsOn clause for reasourceId

\- Create storage account specify resource group location, sku and kind

\- Create NSG and add a securityRules into properties section for
inbound RDP

\- Create virtual machine with ***dependsOn*** clause to storage
account. In properties, ***hardwareProfile*** -size of VM,
***osProfile***- admin username/password, ***storageProfile***-
imageReference, ***osDisk***, ***dataDisks***, ***networkProfile***-
attach network interface with ***<u>resourceId</u>*** function,
***diagnosticProfile***- enable boot diagnostics and link storage
account with ***storageUri***

\- You can deploy ARM template using template deployment in Azure

**Modularize templates**

\- Sometimes your templates can become really large because of the
number of resources that need to be deployed. It is difficult in
maintainability perspective to put all resources onto a template itself

\- In this case, you can break the template into multiple pieces where
you can create ***nested*** or ***linked*** templates

\- Here the definition of the nested resource is defined within the main
template

\- Other way is define your resource in another template and link it
pairing template. There is concept called modules for linked template

***Deployment mode***

Incremental mode - Here resources defined in the template are deployed.
It does not interfere with other resources defined in the resource group
which are not defined in the template.

Complete mode - The resources defined in the template will only be
defined in the resource group. If there are other resources in the
resource group that are not managed by ARM template, they will be
deleted

\- For nested and linked templates, incremental mode is the only mode
that can use

**Nested template**

\- One template remains inside another template

\- In this case, we connect Azure Web app with Azure SQL database

\- For that create new template and copy content of web app template.
Add type ***Microsoft.Resources/deployments*** after web app content,
add ***mode*** as incremental in properties. Then add Azure SQL database
template schema, content version and resources section

\- Add parameters from SQL database template and add into nested
template

\- Deploy resource using template deployment in Azure

{

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"contentVersion": "1.0.0.0",

"parameters": {

"SQLLogin": {

"type":"string",

"metadata":{

"description":"The administrator user name"

}

},

"SQLPassword": {

"type":"secureString",

"metadata":{

"description":"The administrator password"

}

}

},

"functions": \[\],

"variables": {},

"resources": \[

{

"type": "Microsoft.Web/serverfarms",

"apiVersion": "2022-03-01",

"name": "plan787878",

"location": "\[resourceGroup().location\]",

"sku": {

"name":"F1",

"capacity":1

},

"properties":{

"name":"plan787878"

}

},

{

"type": "Microsoft.Web/sites",

"apiVersion": "2022-03-01",

"name": "newapp994848",

"location": "\[resourceGroup().location\]",

"properties":{

"name":"newapp994848",

"serverFarmId":"\[resourceId('Microsoft.Web/serverfarms','plan787878')\]"

},

"dependsOn":\[

"\[resourceId('Microsoft.Web/serverfarms','plan787878')\]"

\]

},

{

"type":"Microsoft.Resources/deployments",

"apiVersion":"2021-04-01",

"name":"childTemplate",

"properties": {

"mode": "Incremental",

"template": {

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"contentVersion": "1.0.0.0",

"resources": \[

{

"type": "Microsoft.Sql/servers",

"apiVersion": "2022-02-01-preview",

"name": "sqlserver500505",

"location": "\[resourceGroup().location\]",

"properties":{

"administratorLogin": "\[parameters('SQLLogin')\]",

"administratorLoginPassword": "\[parameters('SQLPassword')\]"

}

},

{

"type": "Microsoft.Sql/servers/databases",

"apiVersion": "2022-02-01-preview",

"name": "\[format('{0}/{1}','sqlserver500505','appdb')\]",

"location": "\[resourceGroup().location\]",

"sku":{

"name":"Basic",

"tier":"Basic"

},

"properties":{},

"dependsOn":\[

"\[resourceId('Microsoft.Sql/servers','sqlserver500505')\]"

\]

}

\]

}

}

}

\],

"outputs": {}

}

**Linked template**

\- Create new template file in a folder linkedtemplate with default ARM
structure in VS code

\- Copy resource section of Azure web app and app service plan on to new
template file (main.json)and make slight change on name of web app and
app service plan( This should do as Azure portal pop up error when you
recreate resources with same name that you repeatedly use)

\- Copy resource section of database server and database on to new
template file(sqldatabase.json) in the folder linkedtemplate and make
slight change on name of database server and database

\- After resource section on main.json file, add type
***Microsoft.Resources/deployments*** after web app content, apiVersion,
the name-templateLink and mode- incremental and ***templateLink*** in
properties where we upload database template file onto blob container in
Azure storage account and mention URL of template file on uri in
***templateLink*** so that create a storage account with allowing blob
anonymous access and a blob inside the storage account, then upload the
database template file(sqldatabase.json) and get URL of the uploaded
file, paste the URL in ***templateLink***, mention content version after
uri

\- To define database parameters, we should create a new
template(sqldatabase-parameters.json) in the folder linkedtemplate and
specify SQLLogin and SQLPassword in parameters section. The upload the
file to blob in the storage account

\- Add ***parametersLink*** after ***templateLink*** section in
main.json file to link parameter through file uploaded to blob and
mention URL of template file on uri in ***parametersLink,*** , mention
content version after uri

\- Finally deploy resources through main template using template
deployment in Azure portal

**Release pipelines- ARM Templates**

\- Refer the release pipeline created earlier to create SQL table and
insert data into the database using Inline SQL script that manually
created

\- Add template files(main.json, sqldatabase.json,
sqldatabase-parameters.json) also onto blob container in the storage
account

\- Add following tasks into agent job in release pipeline in sequence.

1\. ***ARM template deployment*** task specify Azure Resource Manager
connection, subscription, action- create and update resource group,
resource group(create a RG first), location, template location(it could
be ***Linked artifact*** or ***URL of the file***), Template link- we
choose URL for the file and specify URL of main template file(main.json)
in storage account, Deployment mode- Incremental

2\. Create ***Azure SQL database deployment*** task to create a table
and insert data into the table. In that task, specify display name,
Azure SQL server(Change the SQL server name as per the SQL template or
we may pass down values from ARM template deployment task to subsequent
tasks), database name, login credentials to DB, Deploy type- Inline SQL
script, insert the inline SQL script for table creation, Firewall-
specify firewall rules using ***IPAddressRange***, Start IP address and
end IP address is 0.0.0.0

3\. Create ***Azure Web App*** task to specify app type and application
name and deploy onto Azure Web App where it needs to change the Azure
web app name as per template value

4\. Add ***Azure App Service Setting***s task specifying Azure App
service name, resource group and connection string(add database server
name into connection string). It needs to change the Azure web app name
as per template value

\*\*If we make change on code and commit, it starts to trigger build
pipeline and release pipeline where it doesn't create the resources
again that define in ***ARM template deployment*** task and execute the
remaining tasks

**Release pipeline - Deleting resources**

\- Apart from creating resources into resource group as part of release
pipeline, deleting resources can also be done as part of release
pipeline

\- Once resources are deployed to test environment and testing is
complete, they can be deployed to staging environment after deleting
resources in testing environment

\- Create a script to delete resources using Azure CLI command. Thus,
you can delete each resource using Azure CLI

az resource delete -g template-grp -n "sqlserver700505/appdb"
--resource-type "Microsoft.Sql/servers/databases"

\- Add a new stage to deploy resources to staging environment and add
***Azure CLI*** task to delete resources from testing environment where
specify Azure Resource Manager connection, script type- PowerShell,
script location - Inline script

\- Enable post deployment approvals on testing environment stage to get
approval prior to delete resources in testing environment at staging
environment stage

\*\* When you deploy resources in multiple environments such as
development, test, staging and production, names of resources can change
dynamically through parameters file and pass the value as parameters

**Release pipeline- ARM template artifacts**

\- Previously ***ARM template deployment*** task gets the ARM template
files from ***URL of the file*** in storage account that stored

\- Thus, ***ARM template deploymen***t task can define template location
as ***Linked artifact*** where we upload main ARM template file into
repository as part of code base from Visual Studio by making a new
folder and adding main.json file into cloned repository from Azure
Repos. Then commit and push the repository, it trigger the build
pipeline and subsequently release pipeline.

\- Before build pipeline triggers, change build pipeline by adding a
***PublishPipelineArtifact*** task to YAML file to publish pipeline
artifact and to take ARM template file added into template folder in
source code which is after the task of publishing pipeline artifact to
release pipeline.

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.ArtifactStagingDirectory)'

artifactName: 'sqlapp-artifact'

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.SourcesDirectory)/sqlapp/Templates'

artifactName: 'template-artifact'

\* ***Build.SourcesDirectory*** is a predefined variable that is the
local path on the agent where your source code files are downloaded
c:\agent_work\1\s

\- Then change template location in release pipeline as ***Linked
artifact*** and browse main.json ARM template file from published
artifact in 'template-artifact'

\- Commit changes to code repository which triggers build pipeline and
release pipeline subsequently.

**ARM Templates - Dynamic Resource creation**

\- This is where the method how dynamically change name of resources

\- Use variables in ARM template to dynamically define name of resources

“variables”: {

“sql-server-name”:”concat(‘server’,uniqueString(resourceGroup().id))\]”

}, ; this takes unique string from resource group and concatenating to
server string

"resources": \[

{

"type": "Microsoft.Sql/servers",

"apiVersion": "2022-02-01-preview",

"name": "\[variables('sql-server-name')\]",

"location": "\[resourceGroup().location\]",

"properties":{

"administratorLogin": "\[parameters('SQLLogin')\]",

"administratorLoginPassword": "\[parameters('SQLPassword')\]"

}

},

{

"type": "Microsoft.Sql/servers/databases",

"apiVersion": "2022-02-01-preview",

"name": "\[format('{0}/{1}',variables('sql-server-name'),'appdb')\]",

"location": "\[resourceGroup().location\]",

"sku":{

"name":"Basic",

"tier":"Basic"

},

"properties":{},

"dependsOn":\[

"\[resourceId('Microsoft.Sql/servers',variables('sql-server-name'))\]"

\]

}

\- Define variable use in all place in name of resources,
\[variables('sql-server-name')\]

\- To define output values for SQL server in ARM template, get FQDN of
resource name and pass to subsequent tasks of release pipeline.

"outputs": {

"sqlserverfqdn": {

"type": "string",

"value":"\[reference(variables('sql-server-name')).fullyQualifiedDomainName\]"

}

}

\- Define variable in main ARM template for web app

\- To get web app name to subsequent task, define output values for web
app name and SQL server name that reference from ***templateLink***
through main.json

"outputs": {

"webappname": {

"type": "string",

"value":"\[variables('web-app-name')\]"

},

"sqlserverfqdn": {

"type": "string",

"value":"\[reference('LinkedTemplate').outputs.sqlserverfqdn.value\]"

}

}

\- Create resources using template deployment in Azure which create
Azure web app and database server with dynamic names.

\- You can see value of outputs specified at output section in
deployment in Azure

\- You can manually add variables as part of pipeline externally by
selecting settable at release time. Then write a PowerShell script to
extract the output values that return from ARM template and pass those
values to the variable that you defined as external variables. You
should store the PowerShell script in a folder in main source code
project and commit changes to Azure Repos.

param (

\[Parameter(Mandatory=\$true)\]\[string\]\$ARMValues

)

Write-Host "Starting the script"

\$outputs = \$ARMValues \| convertfrom-json

foreach (\$output in \$outputs) {

\$value1=\$output.'webappname'.value

\$value2=\$output.'sqlserverfqdn'.value ; extracts outputs as JSON
format

Write-Host \$value1

Write-Host \$value2

Write-Host "##vso\[task.setvariable variable=webappname;\]\$value1"

Write-Host "##vso\[task.setvariable variable=sqlserverfqdn;\]\$value2" ;
set the value extracted on variables created

}

\- Before release pipeline triggers, add random string
'resourcesdeployed' onto ***Deployment outputs*** in ***ARM template
deployment*** task where it extracts output of ARM template as JSON
format and set the variables accordingly

-Add PowerShell script into template folder in source code

\- Then add ***PowerShell*** task after ***ARM template deployment***
task by browsing script in script path and pass deployment outputs
'resourcesdeployed' to variable \$ARMValues through Arguments
***-ARMValues ‘\$(resourcesdeployed)’***

\- To verify the values extracted from Deployment outputs are set up
correctly in variables, so you need to create ***Bash script*** task
with inline type as follows after ***PowerShell***

echo “Server name is \$(sqlserverfqdn)”

echo “Web app name is \$(webappname)”

\- Then replace variables set up as part of release pipeline in the
***Azure SQL Database deployment, Azure Web App, Azure App Service
Settings*** tasks with the echoes variable.

**Deploying resources via Azure CLI**

\- Run the following commands one by one on cloud shell

az appservice plan create -g template-grp -n plan787878 --sku F1 --l
"North Europe"

az webapp create -g template-grp -p plan787878 -n newapp1094848
--runtime "dotnet:6"

az webapp list-runtimes ; list the runtime available

az sql server create --name sqlserver420505 --resource-group
template-grp --location "North Europe" --admin-user sqlusr
--admin-password Azure@123

az sql db create --resource-group template-grp --server sqlserver420505
--name appdb --service-objective "Basic"

\- Run Azure CLI commands to create resource which provides json output
for status of resource creation

**Release pipeline- Azure CLI**

\- Clone a pipeline from existing release pipeline, remove ***ARM
template deployment, PowerShell and Bash script tasks***

\- It clones the artifact as well where you should change the artifact
on release accordingly. Otherwise, it will trigger the releases that
have same artifact if build pipeline and release connects through
continuous integration.

\- Add ***Azure CLI*** tasks for Azure Web App and Azure SQL Database by
specifying Azure Resource Manager connection, script type - PowerShell,
script location - Inline script, copy Azure CLI commands

az appservice plan create -g template-grp -n plan787878 --sku F1 --l
"North Europe"

az webapp create -g template-grp -p plan787878 -n newapp1094848
--runtime "dotnet:6"

az webapp list-runtimes ; list the runtime available

az sql server create --name sqlserver420505 --resource-group
template-grp --location "North Europe" --admin-user sqlusr
--admin-password Azure@123

az sql db create --resource-group template-grp --server sqlserver420505
--name appdb --service-objective "Basic"

**Terraform**

\- Infrastructure as code solution that similar to ARM template

\- An open-source tool developed by HashiCorp

\- It helps to automate and manage your infrastructure

\- It uses a declarative language to define the code

\- Deploy and configure your infrastructure

\- Change the code whenever you required

\- Share the code and make versioning of the code

\- It works with variety of cloud providers

\- The code is human readable

1\. Write your Terraform configuration file - You define the resources
that need to be deployed in the configuration file

2\. Terraform plan - Terraform looks at the configuration file and
decides what needs to be deployed. It actually maintains a state file

3\. Terraform apply - Apply all of the changes as per the Terraform
configuration file

\- We use Terraform CLI, download Terraform binary file to your local
machine, you develop your configuration file, plan and apply
configuration file accordingly

**Installing Terraform**

\- Download Terraform AMD64 latest version

\- Extract zip downloaded file to directory in C

\- Add the path to environment variables

\- Check the terraform version from the directory

\- Add extensions Hashicorp Terraform and Azure Terraform on to VS code

\- Open the Terraform folder from VS code and create new file .tf
extension which identify terraform file by VS code

**Creating resources via Terraform**

1\. Specify the version of the AzureRM provider to use

terraform {

required_providers { ; resource provider

azurerm = {

source="hashicorp/azurerm"

version="3.17.0"

}

}

}

2\. Configure AzureRM provider- This is how provider connect to Azure
account. Register terraform app(service principal) on Entra ID and
collect client ID. Generate a client secret with expiration date and
copy the value. These values are required for configuration files to
connect Azure and create resources. We need to provide contributor
access permission to the application created in the subscription through
role assignment to the subscription

/

3\. Define resource blocks.

resource "azurerm_service_plan" "plan787878" {

name = "plan787878"

resource_group_name = "template-grp"

location = "North Europe"

os_type = "Windows"

sku_name = "F1"

}

resource "azurerm_windows_web_app" "newapp1002030" {

name = "newapp1002030"

resource_group_name = "template-grp"

location = "North Europe"

service_plan_id = azurerm_service_plan.plan787878.id

site_config {

always_on = false ; since the SKU is free tier

application_stack{

current_stack="dotnet"

dotnet_version="v6.0"

}

}

depends_on = \[

azurerm_service_plan.plan787878

\]

}

resource "azurerm_mssql_server" "sqlserver468985656" {

name = "sqlserver468985656"

resource_group_name = "template-grp"

location = "North Europe"

version = "12.0"

administrator_login = "sqlusr"

administrator_login_password = "Azure@123"

}

resource "azurerm_mssql_database" "appdb" {

name = "appdb"

server_id = azurerm_mssql_server.sqlserver468985656.id

collation = "SQL_Latin1_General_CP1_CI_AS"

license_type = "LicenseIncluded"

max_size_gb = 2

sku_name = "Basic"

depends_on = \[

azurerm_mssql_server.sqlserver468985656

\]

}

\- Deploy resources that define in configuration file from visual studio
itself so that go to terminal which will open up PowerShell

terraform init ; this will download azurerm provider plugin and modules
that required to interact with Azure terraform Configure file

terraform plan -out main.tfplan ; this will create plan file where it
compares what resources are included in Azure account against what we
need to deploy using main config file. Also it provides properties for
the resources that we deploy

terraform apply “main.tfplan” ; deploy the resources

terraform destroy ; delete the resources. It needs to provide permission
to delete resources

**Release pipeline- Terraform**

\- Add main.tf file into template folder in source code

\- Commit the template folder to remote repository in Azure Repos

\- Once commit the changes, it starts to trigger build pipeline

\- Before creating release pipeline, it needs to install terraform tool
extension in Azure DevOps organization from the market place so that
tasks relate to terraform tasks are available for releases

\- Then you can add tasks that ***Terraform tool installer*** -
version(latest )and ***Terraform*** - execute terraform commands to
manage on AzureRM

\- In ***Terraform*** task, provide display name, provider: azurerm,
command: init, configuration directory- add path for template folder
that consists terraform configuration file(main.tf), choose Azure
subscription, resource group, choose storage account to store terraform
state file, name of the blob container in storage and terraform state
file(terraform.tfstate)\* The container should have anonymous access
enabled

\- Thus add ***Terraform*** tasks for plan and apply into release
pipeline. In apply task, add ***Additional command arguments*** as
-auto-approve

\- Specify the Azure Web App name and Azure SQL server name in the tasks
release pipeline in the ***Azure SQL Database deployment, Azure Web App,
Azure App Service Settings*** in release pipeline

\- Create release pipeline to trigger the pipeline

**Azure Release Pipeline - YAML - Azure CLI**

\- This is an example how you can extend YAML build pipeline to release
pipeline as build pipeline comes with YAML and release pipeline comes
with UI interface

-Inherently, build pipeline is part of a stage and job

\- To extend build pipeline, add new stages/job for build and deploy and
download published artifact from artifact staging directory

\- Get YAML definition of each task in release pipeline, select ***view
YAML*** and add the YAML output of each task into build YAML pipeline
along with mandatory indentation

-Add ***Azure SQL Database deployment, Azure Web App, Azure App Service
Settings*** tasks in YAML format into YAML pipelines

-Make sure to use same name of published artifact when it downloads into
deploy stage

-Validate the whole YAML definition when it is ready to deploy using
build pipeline. The validate result shows OK

-Grant permission that will permit the use of service connection for all
waiting and future runs of the pipeline in order to move to deploy stage

-Commit change to trigger the build pipeline

trigger:

\- main

resources:

\- repo: self

pool:

vmImage: 'windows-latest'

variables:

solution: '\*\*/\*.sln'

buildPlatform: 'Any CPU'

buildConfiguration: 'Release'

stages:

\- stage: Build

displayName: Build stage

jobs:

\- job: Build

displayName: Build

steps:

\- task: NuGetToolInstaller@1

\- task: NuGetCommand@2

inputs:

restoreSolution: '\$(solution)'

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: DotNetCoreCLI@2

inputs:

command: publish

publishWebProjects: True

arguments: '--configuration \$(BuildConfiguration) --output
\$(Build.ArtifactStagingDirectory)'

zipAfterPublish: True

\# We still need to take the staging directory files and publish it as a
build artifact

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.ArtifactStagingDirectory)'

artifactName: 'sqlapp-secure-artifact'

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.SourcesDirectory)/sqlapp/Templates'

artifactName: 'template-artifact'

\- stage: Deploy

displayName: Deployment stage

jobs:

\- job: Deploy

displayName: Deploy

steps:

\- download: current

artifact: sqlapp-secure-artifact

\- task: AzureCLI@2

displayName: 'Azure CLI - Azure Web App'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

scriptType: ps

scriptLocation: inlineScript

inlineScript: \|

az appservice plan create -g template-grp -n plan787878 --sku F1 --l
"North Europe"

az webapp create -g template-grp -p plan787878 -n newapp3094848
--runtime "dotnet:6"

\- task: AzureCLI@2

displayName: 'Azure CLI - Azure SQL Database'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

scriptType: ps

scriptLocation: inlineScript

inlineScript: \|

az sql server create --name sqlserver4205058 --resource-group
template-grp --location "North Europe" --admin-user sqlusr
--admin-password Azure@123

az sql db create --resource-group template-grp --server sqlserver4205058
--name appdb --service-objective "Basic"

\- task: SqlAzureDacpacDeployment@1

displayName: 'Azure SQL Table creation'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

ServerName: sqlserver4205058.database.windows.net

DatabaseName: appdb

SqlUsername: sqlusr

SqlPassword: 'Azure@123'

deployType: InlineSqlTask

SqlInline: \|

IF (NOT EXISTS (SELECT \*

FROM INFORMATION_SCHEMA.TABLES

WHERE TABLE_SCHEMA = 'dbo'

AND TABLE_NAME = 'Products'))

BEGIN

CREATE TABLE Products

(

ProductID int,

ProductName varchar(1000),

Quantity int

)

INSERT INTO Products(ProductID,ProductName,Quantity) VALUES
(1,'Mobile',100)

INSERT INTO Products(ProductID,ProductName,Quantity) VALUES
(2,'Laptop',200)

INSERT INTO Products(ProductID,ProductName,Quantity) VALUES
(3,'Tabs',300)

END

IpDetectionMethod: IPAddressRange

StartIpAddress: 0.0.0.0

EndIpAddress: 0.0.0.0

DeleteFirewallRule: false

\- task: AzureWebApp@1

displayName: 'Azure Web App Deploy: newapp3094848'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

appType: webApp

appName: newapp3094848

Package: '\$(Pipeline.Workspace)/sqlapp-secure-artifact/\*\*/\*.zip'

\- task: AzureAppServiceSettings@1

displayName: 'Azure App Service Settings: newapp3094848'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

appName: newapp3094848

resourceGroupName: 'template-grp'

connectionStrings: \|

\[

{

"name": "SQLConnection",

"value": "Server=tcp:sqlserver4205058.database.windows.net,1433;Initial
Catalog=appdb;Persist Security Info=False;User
ID=sqlusr;Password=Azure@123;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection
Timeout=30;",

"type": "SQLAzure",

"slotSetting": false

}

\]

**Azure Release Pipelines - YAML - ARM Templates**

\- This extends build pipeline for provisioning resources through ARM
template

\- add new stage for deploy and add ***download*** task for pipeline
artifact, template artifact that added into main project, add task for
checking the data within pipeline workspace

\- Then add task ***ARM template deploymen***t which have YAML output
format

\- Get ***view YAML*** of task in release pipeline and add the YAML
output for the tasks into build pipeline along with mandatory
indentation

-Add ***Azure SQL Database deployment, Azure Web App, Azure App Service
Settings*** tasks in YAML format into YAML pipelines

-Make sure to use same name of published artifact when it downloads into
deploy stage

-Validate the whole YAML definition when it is ready to deploy using
build pipeline. The validate result shows OK

-Commit change to trigger the build pipeline

trigger:

\- main

pool:

vmImage: 'windows-latest'

resources:

\- repo: self

variables:

solution: '\*\*/\*.sln'

buildPlatform: 'Any CPU'

buildConfiguration: 'Release'

stages:

\- stage: Build

displayName: Build stage

jobs:

\- job: Build

displayName: Build

steps:

\- task: NuGetToolInstaller@1

\- task: NuGetCommand@2

inputs:

restoreSolution: '\$(solution)'

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: DotNetCoreCLI@2

inputs:

command: publish

publishWebProjects: True

arguments: '--configuration \$(BuildConfiguration) --output
\$(Build.ArtifactStagingDirectory)'

zipAfterPublish: True

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.ArtifactStagingDirectory)'

artifactName: 'sqlapp-artifact'

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.SourcesDirectory)/sqlapp/Templates'

artifactName: 'template-artifact'

\- stage: Deploy

displayName: Deployment stage

jobs:

\- job: Deploy

displayName: Deploy

steps:

\- download: current

artifact: sqlapp-artifact

\- download: current

artifact: template-artifact

\- pwsh: \|

Get-ChildItem -Path \$(Pipeline.Workspace)\\.\* -Recurse -Force \|
Out-String -Width 180

errorActionPreference: continue

displayName: 'List content'

continueOnError: true

\- task: AzureResourceManagerTemplateDeployment@3

displayName: 'ARM Template deployment: Resource Group scope'

inputs:

azureResourceManagerConnection: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

subscriptionId: '6912d7a0-bc28-459a-9407-33bbba641c07'

resourceGroupName: 'template-grp'

location: 'North Europe'

csmFile: '\$(Pipeline.Workspace)/template-artifact/main.json'

action: 'Create Or Update Resource Group'

deploymentMode: 'Incremental'

\- task: SqlAzureDacpacDeployment@1

displayName: 'Azure SQL InlineSqlTask'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

ServerName: sqlserver8000505.database.windows.net

DatabaseName: appdb

SqlUsername: sqlusr

SqlPassword: 'Azure@123'

deployType: InlineSqlTask

SqlInline: \|

IF (NOT EXISTS (SELECT \*

FROM INFORMATION_SCHEMA.TABLES

WHERE TABLE_SCHEMA = 'dbo'

AND TABLE_NAME = 'Products'))

BEGIN

CREATE TABLE Products

(

ProductID int,

ProductName varchar(1000),

Quantity int

)

INSERT INTO Products(ProductID,ProductName,Quantity) VALUES
(1,'Mobile',100)

INSERT INTO Products(ProductID,ProductName,Quantity) VALUES
(2,'Laptop',200)

INSERT INTO Products(ProductID,ProductName,Quantity) VALUES
(3,'Tabs',300)

END

IpDetectionMethod: IPAddressRange

StartIpAddress: 0.0.0.0

EndIpAddress: 0.0.0.0

DeleteFirewallRule: false

\- task: AzureRmWebAppDeployment@4

displayName: 'Azure App Service Deploy'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

WebAppName: newapp1094848

Package: '\$(Pipeline.Workspace)/sqlapp-artifact/\*\*/\*.zip'

\- task: AzureAppServiceSettings@1

displayName: 'Azure App Service Settings: newapp1094848'

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

appName: newapp1094848

resourceGroupName: 'template-grp'

connectionStrings: \|

\[

{

"name": "SQLConnection",

"value": "Server=tcp:sqlserver8000505.database.windows.net,1433;Initial
Catalog=appdb;Persist Security Info=False;User
ID=sqlusr;Password=Azure@123;MultipleActiveResultSets=False;Encrypt=True;TrustServerCertificate=False;Connection
Timeout=30;",

"type": "SQLAzure",

"slotSetting": false

}

\]

**Desire State Configuration**

\- Assume a machine has tools or software installed support the
application such as IIS for Web application

\- It has to be ensured that the configuration of the machine doesn’t
not drift or it could be impact the application, for this you can make
use of ***PowerShell DSC***

\- PowerShell DSC can be implemented by using server that is called
Azure automation DSC which is inbuilt server that ensures all machines
receive the desired configuration

\- You can manage all configuration and nodes from Azure portal itself

**Lab - Azure automation DSC**

Azure automation is used for configuration management, update
management, integration and process automation.

\- Create a new VM by exposing port 80(With DSC we ensure IIS role is
present on VM)

\- Create an Automation account in Azure by specifying name, region

\- Install IIS feature on the VM through automation account using
PowerShell DSC. This is done using PowerShell script file as follows.

configuration NewConfig ; name of configure

{

Node localhost ; node is local server

{

WindowsFeature IIS

{

Ensure = 'Present'

Name = 'Web-Server'

IncludeAllSubFeature = \$true

}

}

}

\- Upload configuration file onto configuration section into Automation
Account, Automation Account \> State configuration(DSC) \> Configuration
\> Add(browse the script by adding name)

\- Compile the configuration which submit a compilation job for script.
Once compilation is complete, it shows Node
Configuration(***NewConfig.localhost***) in ***Compiled configuration***
section after 1 minute time

\- Onboard VMs into automation account where an extension is installed
on the VM which allows VM to communicate with automation account.
Automation Account \> State configuration(DSC) \> Nodes \> +Add(It shows
available VMs) \> Select the VM \> Connect(It goes to registration
process of VM)

Registration key- primary key

Node configuration name- name of configuration
added(***NewConfig.localhost***)

Refresh frequency- the frequency that PowerShell DSC local configuration
manager contacts the Azure Automation DSC pull server to download the
latest node configuration(the interval that Azure automation will keep
on checking whether configuration applies on the machine)

Configuration Mode frequency - the frequency that the background
application of DSC attempts to implement the current node configuration
on the target node

Configuration mode -
ApplyAndAutoCorrect(ApplyAndAutoCorrect/ApplyOnly/ApplyAndMonitor) - it
ensures that the configuration applies again if there is configuration
drift

Allow Module Override - Check the box

Reboot Node if Needed - Check the box

Action after Reboot - ContinueConfiguration

-This registration process will install extension on the VM which allows
to communicate the VM with Automation account

-You can see ***Microsoft.PowerShell.DSC*** extension is available on
Extension + application on Azure AM

-You can check the default IIS web page through the public IP address of
VM through web browser

\- Once VM connects to Azure automation account, the node configuration
status will be compliant.

\- When you uninstall web server feature forcefully and reboot the
server manually, the IIS feature will be reinstalled after refresh
frequency by Azure automation DSC

**File DSC resource**

\- When you want to ensure particular file should be present on
***SourcePath*** from pull server to ***DestinationPath*** to VM

\- Thus you can ensure to place file, group, log, package, registry,
script and so on.

**Using VM extension**

**Custom Script Extension**

\- The extension can be used to download and run scripts on the Azure
virtual machine

\- Assume once you create a VM, you need to ensure a software
automatically gets installed on the VM so that you can use Custom Script
Extension for post-deployment configuration or software installation

let’s consider the scenario.

\- Register the machine with a deployment group - Use Team Services
Agent

\- Install Internet Information Services and ASP.NET hosting bundle -
Use Custom Script Extension

**Lab - Team Services Agent**

Team service agent extension is used to run registration script on
virtual machine.

\- To connect VM that creates using ARM template into deployment group,
we install ***TeamServicesAgent*** extension on VM instead of CSE where
the extension run registration script that needs to register VMs into
deployment group. We specify Azure DevOps organization, name of team
project, name of deployment group, agent name and personal access token
with scopes for deployment group in properties in the ARM template

-Use template deployment in Azure to create a VM with registration
script run using ***TeamServicesAgent***

-You can see ***TeamServicesAgent*** extension is available on
Extension + application on Azure AM

-You can see ***appvm*** places in targets in deployment group

"name": "appvm",

"type": "Microsoft.Compute/virtualMachines",

"apiVersion": "2021-03-01",

"location": "\[resourceGroup().location\]",

"resources": \[

{

"name": "\[concat('appvm','/TeamServicesAgent')\]",

"type": "Microsoft.Compute/virtualMachines/extensions",

"location": "\[resourceGroup().location\]",

"apiVersion": "2021-03-01",

"dependsOn": \[

"\[resourceId('Microsoft.Compute/virtualMachines/','appvm')\]"

\],

"properties": {

"publisher": "Microsoft.VisualStudio.Services",

"type": "TeamServicesAgent",

"typeHandlerVersion": "1.0",

"autoUpgradeMinorVersion": true,

"settings": {

"VSTSAccountName": "techsup4000",

"TeamProject": "DevProject",

"DeploymentGroup": "Web Servers",

"AgentName": "appvm"

},

"protectedSettings": {

"PATToken": "v3d3u7sfeawsn6cdb7pqfyfmnjx7ozsewv464s7jmheeosogrpsa"

}

}

}

\],

"dependsOn": \[

"\[resourceId('Microsoft.Storage/storageAccounts',
toLower('vmstore8677676'))\]"

\],

**Lab - Custom Script Extension**

\- Create custom PowerShell script to install IIS feature and ASP.NET
hosting bundle where executable file of ASP.NET hosting bundle is
uploaded to blob container that has anonymous access, then specify the
URL of uploaded executable file of .NET hosting bundle in \$Url in the
script

Install-WindowsFeature -name Web-Server -IncludeManagementTools

Write-Output "Installed IIS"

New-Item -Path "D:\\ -Name "tmp" -ItemType "directory"

\$Path = "D:\tmp\\

\$Url =
"<https://templatestore465656.blob.core.windows.net/installers/dotnet-hosting-6.0.8-win.exe>"

\$Location = \$Path + \[System.IO.Path\]::GetFileName(\$Url)

Invoke-WebRequest -Uri \$Url -OutFile \$Location

Start-Process -FilePath \$Location -Wait -ArgumentList /passive

net stop was /y

net start w3svc

Write-Output "Installed Hosting Bundle"

\- Upload the custom script also into blob container

\- ***Generate SAS*** for the PowerShell script and paste Blob SAS URL
in ***fileUris*** section in CSE section in ARM template that used to
create VM that has been already registered with deployment group

"type": "Microsoft.Compute/virtualMachines/extensions",

"name": "\[concat('appvm', '/config-app')\]",

"location": "\[resourceGroup().location\]",

"apiVersion": "2018-06-01",

"dependsOn": \[

"\[resourceId('Microsoft.Compute/virtualMachines/', 'appvm')\]"

\],

"properties": {

"publisher": "Microsoft.Compute",

"type": "CustomScriptExtension",

"typeHandlerVersion": "1.10",

"autoUpgradeMinorVersion": true,

"settings": {

"fileUris": \[

"<https://templatestore465656.blob.core.windows.net/installers/script.ps1?sp=r&st=2022-08-13T16:32:07Z&se=2022-08-14T00:32:07Z&spr=https&sv=2021-06-08&sr=b&sig=Hzmg4K%2F7A4QnEXlQz7LZliJW1%2BXLOzXDfHuBKd8V1b8%3D>"

\],

"commandToExecute": "powershell -ExecutionPolicy Unrestricted -File
script.ps1"

}

}}

\],

"outputs": {}

\- Deploy the ARM template using template deployment where ARM template
only install IIS and .NET hosting bundle because the ARM template use
deployment mode -Incremental

\*\*We can create release pipeline with following tasks to deploy .NET
web app

1.  ARM Template deployment task - Create VM and register the VM to
    deployment group using ***TeamServiceAgent***

2.  ARM Template deployment task - Install IISand ASP.NET hosting bundle
    using CSE

3.  IIS Web app Manage

4.  IIS Web app Deploy

**Virtual Machine Scale Sets(VMSS)**

\- VMSS use to increase and decrease the number of VMs how demand
fluctuates based on condition - metrics

-The load of VMs might increase when number of users access VMs increase

**ARM Template -** **Virtual Machine Scale Sets**

\- We can use ARM template to create VMSS where it includes these
section.

Load balancer - distribute traffic in VMSS

Public IP address - for load balancer

Backend pool

Load balancing rule for backend pool, protocol, specify frontend and
backend port number, configure health probe

Virtual Machine Scale Sets - Number of VMs, size VM, upgradepolicy,
osprofile, networkprofile, virtual network for VMs

-Deploy the ARM template using template deployment in Azure

**ARM Template - Virtual machine scale set extension**

\- Use ARM template to deploy ***TeamServiceAgent*** to register VM
instances in VMSS with deployment group and custom script extension to
install IIS feature and ASP.NET hosting bundle on instances in VMSS

\- In ARM template, use extension profile to include all extensions
require

"extensionProfile": {

"extensions": \[

{

"type": "Microsoft.Compute/virtualMachineScaleSets/extensions",

"name": "TeamServicesAgent",

"location": "\[resourceGroup().location\]",

"properties": {

"publisher": "Microsoft.VisualStudio.Services",

"type": "TeamServicesAgent",

"typeHandlerVersion": "1.0",

"autoUpgradeMinorVersion": true,

"settings": {

"VSTSAccountName": "techsup4000",

"TeamProject": "AgileProject",

"DeploymentGroup": "Agile-Deployment"

},

"protectedSettings": {

"PATToken": "hhcfq24jvjgi7g6xjzlgfhr2boz2gdkxuxfjkgt5vpd4sffsfp3a"

}

}

},

{

"type": "Microsoft.Compute/virtualMachineScaleSets/extensions",

"name": "config-app",

"location": "\[resourceGroup().location\]",

"properties": {

"publisher": "Microsoft.Compute",

"type": "CustomScriptExtension",

"typeHandlerVersion": "1.10",

"autoUpgradeMinorVersion": true,

"settings": {

"fileUris": \[

"<https://templatestore465656.blob.core.windows.net/installers/script.ps1?sp=r&st=2022-08-17T04:34:28Z&se=2022-08-17T12:34:28Z&spr=https&sv=2021-06-08&sr=b&sig=7OjFWfdeaEg8hzGyfD7BwMzd6CVwXvvcoIlzPfsiMnE%3D>"

\],

"commandToExecute": "powershell -ExecutionPolicy Unrestricted -File
script.ps1"

}

}

}

\]

},

\- Deploy template using template deployment

\- Installing IIS feature and ASP.NET hosting bundle on instances in
VMSS can be done using release pipeline to get more visibility

**VMSS - Application Health Extension**

\- You can monitor the health of individual instances using application
health extension

\- This can be useful when it comes to rolling upgrades for your
instances

\- You can monitor the application health of each instance in scale set
and perform instance repairs

\- Enable ***health and repair*** option and enable automatic repairs,
Virtual Machine Scale Set\> Settings\> Health and repair\> Enable
application health monitoring \> Application health monitor -
Application health extension, Protocol -HTTP, Port number -80, enable
automatic repairs

**Deployments, Packages and Test Plans**

**The fear of changes**

\- Make code changes that need to be deployed when user’s ask for
changes to the application

\- But there is always the fear factor as the application stops working
if the change fails

\- Customers are not happy and also it is risk to the business

\- That’s why companies strive a lot to make manages as seamless as
possible

**Blue-Green Deployments (formerly Red-Black Deployments)**

Blue environment

\- All user traffic is directed to the Blue environment which is the
current production environment

Green environment

\- If a software change needs to be made, then a duplicate environment
is setup and testing on changed application is deployed to this
environment

\- Once sanity check and basic testing is completed, users are then
directed to the Green environment. The Green environment now becomes the
production environment

\- The major concern to deploy change to single environment is the
downtime. If the change wouldn’t work as expected, the downtime will
extend for restoring production environment with backup

-One of the biggest advantage of Blue-Green deployment is quick
switchover users from one environment to other in which downtime is
minimal. Also we can quickly switch back to older version of environment
easily if green environment is not functional as expected.

\- One of the downside of blue-green deployment is cost to maintain
identical environments. However, it depends on how critical the
application is. If the application is about revenue generating, the
minimal downtime is important.

**Azure Web App- Deployment slots**

\- Staging environments for App Service plans

\- Standard, Premium and isolated app service plan have deployment slots
feature, not in free, basic or shared app service plans

\- Deployment slot is like creating entire Azure Web App area which you
can publish newer version of application. When Azure web app creates, it
belongs to production slot by default.

\- Applications in deployment slots have their own host names

\- You have chance to validate all application changes in the staging
deployment slot

\- You can then swap the staging slot with the production slot

\- This helps eliminate the downtime for your application when new
changes are deployed

\- You can also easily roll back the changes by swapping back to
previous production slot

**Lab - Azure Web App- Deployment slots - Manual approach**

\- Create Azure web app with Publish -code, runtime stack .NET 8,
location, app service plan -standard , authentication-basic and disable
application insight

\- Create new project using ASP.NET Core web app template in Visual
Studio 2022

\- Make identifiable change to index.html file and publish the project
into specific target ***Azure app service***, select app service
instance - production deployment slot by creating publish profile

\- Check refreshing the web app name URL in App service on the browser

You can purchase domain from external domain provider and map that
domain to web app name URL in App service

\- Add ***custom domains*** in ***Azure app service*** and validate
where it shows type, host and value for custom domain- ***custom domain
verification ID*** that provides TXT record host and value to verify
domain ownership and CNAME record for subdomain in order to add DNS
configuration portal in external domain provider

\- Then validate the custom domain name for web app after propagate
domain ownership

\- Create custom domain in Azure app service after domain verification
which allows to ***add custom domain*** pointing to CNAME record for
required domain. The create CNAME record for custom domain for DNS of
Azure web app on domain registrar

\- Create new deployment slot naming staging and clone setting from- Do
not clone settings where creates new URL for staging slot. This means
that it creates new web app in the existing App service itself.(\<web
app name\> - staging.azurewebsites.net)

\- Make change on project and publish the project to staging slot by
creating new publish profile

\- Swap the source - staging URL with target- production URL where
changes in staging slot switch the URL of production slot

\- If you face any issue with new version of application, you can swap
back the slot.

**Azure pipeline- Deployment slots**

\- Delete the staging slot from Azure App service

\- Publish the source code by creating git repository in Azure repos by
specifying organization, project and push the project code to Azure
repos

\- Create a build pipeline and publish the build artifact by specifying
***artifactName*** to release pipeline

\- Create release pipeline with an empty job in a stage to deploy into
deployment slot

\- Add artifact that published with build pipeline and enable continuous
deployment trigger

\- Add new stage naming Deployment to slot

\- Add ***Azure CLI*** task to create deployment slot on ***Agent job***
specifying name, Azure Resource Manager connection, script type-
PowerShell, Script Location- Inline script, Inline Script - add Azure
PowerShell command to create deployment slot

az webapp deployment slot create --name deployementapp1000
--resource-group template-grp --slot staging

\- Add ***Azure App Service Deploy*** task to deploy the new change of
web app to staging slot specifying Azure subscription, App service type
-Web App on Windows, app service name, tick ***Deploy to slot or app
service environment***, resource group, slot- staging

\- Enable post deployment approval for the above stage - deployment to
slot

\- Add new stage naming swap slots

\- Add new ***Azure App Service manage*** task to job in stage by
specifying Display name, Azure subscription, Action- swap slot( where it
has many actions), app service name, resource group, slot- staging, tick
***Swap with Production***

\- Add new ***Agentless job*** and add ***Manual intervention*** task in
to the job for conducting sanity check, add instruction for sanity check

\- Add new ***Agent job*** and add ***Azure CLI*** task to delete the
existing staging slot if cost for retaining a slot is a concern

az webapp deployment slot delete --name deployementapp1000
--resource-group template-grp --slot staging

\- Commit the new change to trigger build pipeline and it triggers
release pipeline

-Approve the post deployment approval of stage 1 by checking web app
function

**Canary Deployment**

\- It has production environment where users are directed to the
production environment

\- When a new feature is released for the application onto identical
environment, it is only made available for subset of users

\- You can direct a percentage of users onto duplicate environment that
has new feature

\- After testing the new feature, all of users can gradually move to new
identical environment or you may have an option to toggle feature on and
off within application architecture itself.

\- The solution for the deployment that Azure provides is Azure Traffic
Manager

**Azure Traffic Manager**

\- This is a DNS-based traffic load balancer

\- You can distribute traffic to public facing application across
different Azure regions

\- You can direct traffic based on different routing methods

\- User traffic initially reaches Azure Traffic Manager profile where it
determines how traffic distributes based on routing method

Priority - lowest number of priority will prioritize the traffic directs
to backend endpoints which might be Azure Web App, Azure VMs

Weighted - this is for canary deployment where direct the traffic to
backend endpoints based on weightage. E.g. one backend has weight 1000
and one has 1. All users are directed to backend that has highest
weightage. As long as you increase the weightage of other backend while
decreasing weightage primary backend, traffic manager profile calculates
the percentage based on the weightage and direct the traffic to backend
accordingly

**Lab - Azure Traffic Manager - Manual approach**

\- Create Azure web app in a region as production and publish the code
from VS. Check the URL of web app from browser
([https://deployment.azurewebsites.net](https://deployment.azurewebsites.net/))

\- Create another Azure web app in a different region as staging
environment and create new publish profile to publish the code with new
feature changes. If the Azure web app is not visible on new publish
profile, download publish setting to local machine clicking ***Get
publish profile*** from Azure app service and copy it to temporary
directory. Then select ***Import profile*** in target section on publish
profile to publish code to Azure Web App. Check the URL of web app from
browser
([https://deployment-staging.azurewebsites.net](https://deployment-staging.azurewebsites.net/))

\- Create traffic manager profile specifying name, routing method-
weighted, subscription, resource group where it doesn’t need to specify
location as traffic manager is global resource. DNS name for traffic
manager
([http://deploymentprofile.trafficmanager.net](http://deploymentprofile.trafficmanager.net/))

\- In ***Configuration*** settings on traffic manager profile, change
***Endpoint monitor settings*** to HTTPS and port 443 for SSL
connection, save

\- In ***Endpoints***, add production Azure web app into traffic manager
specifying type-Azure endpoint, name- production, target resource
type-App service, Target- select the Azure web app name for production,
Weight-1000, Custom header settings- host:\<Azure Web App name
-production\>azurewebsites.net. Once it adds, health status of endpoint
will be checked. Thus add staging web app as an endpoint into traffic
manager profile by specifying Weight-1

\- Once monitor status of both backend endpoints are online, check
traffic manager URL. It shows production web app. When we increase
weight of staging web app, user traffic will direct to staging. When
higher number of weight assigns to staging web app, all user traffic
will be directed to staging web app from traffic manager profile

\- While we use priority routing method and when web app with lowest
priority value is degraded, it take 10 minutes time to change monitor
status in endpoints in traffic manager.

\*\*If both endpoint have similar weightage, user traffic distributes to
endpoint similarly.

**Azure Traffic manager - Azure pipeline**

First delete the staging endpoint from traffic manager profile while
both Azure web apps have been already created.

*Stage 1 - Create Traffic Manager endpoint*

Publish new feature change into staging web app

\- Create git repository in Azure repos by specifying organization,
project and push the project code to Azure repos

\- Create build pipeline and publish the build pipeline artifact to
release

\- Create release pipeline with ***Azure App Service Deploy*** task to
deploy the new change to staging web app specifying Azure subscription,
app service name - staging web app

\- Add artifact that build with build pipeline and enable continuous
deployment trigger

Create staging endpoint in traffic manager profile

\- Create ***Azure PowerShell*** task to create staging endpoint
specifying Azure subscription, script type- inline script, write Azure
PowerShell to create endpoint, select latest installed version for Azure
PowerShell version

\- Enable post deployment approval for the stage to verify promoting new
feature to staging Azure Web App and creating traffic manager endpoint

*CreateEndpoint.ps1*

\$TrafficManagerProfileName="deploymentprofile"

\$ResourceGroupName ="template-grp"

\$TargetResourceId="/subscriptions/6912d7a0-bc28-459a-9407-33bbba641c07/resourceGroups/template-grp/providers/Microsoft.Web/sites/deploymentapp1000-staging"

\$TargetEndPoint="deploymentapp1000-staging.azurewebsites.net"

\$TrafficManagerEndpoint = New-AzTrafficManagerEndpoint -Name "staging"
\`

-ProfileName \$TrafficManagerProfileName -Type AzureEndpoints \`

-TargetResourceId \$TargetResourceId -EndpointStatus Enabled \`

-Weight 100 -ResourceGroupName \$ResourceGroupName

Add-AzTrafficManagerCustomHeaderToEndpoint -TrafficManagerEndpoint
\$TrafficManagerEndpoint -Name "host" -Value \$TargetEndPoint

Set-AzTrafficManagerEndpoint -TrafficManagerEndpoint
\$TrafficManagerEndpoint

*Stage 2 -Change Weightage*

Change weightage on endpoints from traffic manager profile

\- Create new stage as naming change weightage

\- Create ***Azure PowerShell*** task to change weightage specifying
Azure subscription, script type- inline script, write Azure PowerShell
to change weightage, select latest installed version for Azure
PowerShell version

*SetEndpint.ps1*

\$TrafficManagerEndpoint = Get-AzTrafficManagerEndpoint -Name
"production" -Type AzureEndpoints -ProfileName "deploymentprofile"
-ResourceGroupName "template-grp"

\$TrafficManagerEndpoint.Weight = 1

Set-AzTrafficManagerEndpoint -TrafficManagerEndpoint
\$TrafficManagerEndpoint

\$TrafficManagerEndpoint = Get-AzTrafficManagerEndpoint -Name "staging"
-Type AzureEndpoints -ProfileName "deploymentprofile" -ResourceGroupName
"template-grp"

\$TrafficManagerEndpoint.Weight = 1000

Set-AzTrafficManagerEndpoint -TrafficManagerEndpoint
\$TrafficManagerEndpoint

\- Make change on web application repository and commit the change to
trigger build and release pipeline

**Using a rolling deployment**

\- When an application runs on set of virtual machines. We have
***deployment group*** in pipeline where change will apply once at a
time on a machine or batches at a time

\- Another version of rolling update is ***Virtual Machine Scale Sets***
where the new feature is deployed to new set of virtual machines and
these machine would replace one machine in existing set of VMs

\- So this is done in rolling fashion across the machines with each
machine being replaced

\- At any point in time, you would have machines the older and newer
application version

**Using a Azure Load Balancer**

We configure these components mainly in Azure load balancer

Backend pool - set of virtual machine that runs application

Health probe - understand if the backend virtual machine are healthy or
not

Load balancing rule- how load balance the incoming traffic from users
across the Azure VMs in backend pool

In blue -green deployment, we can use Azure load balancer as follows.

Blue environment- all users are directed to the current production VMs
using load balancer

Green environment- all users are directed to the environment that deploy
newer version using load balancer

**Lab - Azure load balancer - VM setup**

\- Create new VM as production allowing RDP and HTTP

\- Create another VM as staging allowing RDP and HTTP

\- Install IIS role on production and staging VMs

\- Create html file with simple HTML code and save the file
C:\inetpub\wwwroot on both VMs

\- Check the access to default html file from public IP addresses of VMs
using [http://public IP/deafult.html](http://public%20ip/deafult.html)

\- Before configure Azure load balancer, disassociate public ip
addresses from the VMs because load balancer connect backend VMs from
private IP addresses

**Lab - Azure Load Balancer - Configuration**

\- Create a load balancer specifying name, region, SKU- standard, Type -
public, frontend IP configuration- create new public IP for load
balancer by providing name, create the load balancer first

\- Create 2 ***backed pools*** in load balancer with IP address of the
VM, by specifying name, virtual network, Backend pool configuration - IP
address, IP address- Put IP address of the VM and its resource name

\- Create ***health probe*** to monitor TCP port 80 as IIS service
running with port 80, by specifying Name, Protocol, port, interval

\- Create ***load balancing rules s***pecifying ***frontend IP
address***, select production backend pool, protocol- TCP , port- 80,
backend port - to divert the traffic from frontend to backend, health
probe

-Check the [http://frontend IP of load
balancer/Default.html](http://frontend%20ip%20of%20load%20balancer/Default.html)
and verify the web app on production backend pool

\- Create public DNS that points frontend IP of public load balancer and
you can check web app access from DNS which direct traffic production
backend pool

\- If new feature is deployed to VMs in staging backend pool, you only
need to change backend pool as staging pool in load balancing rule

**Using load balancer- Azure pipeline**

For blue-green deployment, new feature can be tested in staging pool and
switch backend pool from production pool to staging pool

\- Add new release pipeline to demonstrate for swapping backend pool to
staging pool from production after new feature is deployed on to VM in
staging pool

\- Create ***Azure PowerShell*** task in agent job on new stage for
swapping backend pool to staging pool from production by specifying
Azure subscription, script type- inline script, write Azure PowerShell
to swap backend pool, select latest installed version for Azure
PowerShell version

*Script.ps1*

\$ResourceGroupName="load-grp"

\$LoadBalancerName="app-balancer"

\$BackEndPoolName="staging-pool"

\$LoadBalancer = Get-AzLoadBalancer -Name \$LoadBalancerName
-ResourceGroupName \$ResourceGroupName

\$Probe=Get-AzLoadBalancerProbeConfig -Name "probeA" -LoadBalancer
\$LoadBalancer

\$BackendPool = Get-AzLoadBalancerBackendAddressPool -ResourceGroupName
\$ResourceGroupName -LoadBalancerName \$LoadBalancerName -Name
\$BackEndPoolName

\$LoadBalancer \| Set-AzLoadBalancerRuleConfig -Name "RuleA"
-FrontendIPConfiguration \$LoadBalancer.FrontendIpConfigurations\[0\]
-Protocol "Tcp" -FrontendPort 80 -BackendPort 80 -BackendAddressPool
\$BackendPool -Probe \$Probe

\$LoadBalancer \| Set-AzLoadBalancer

\- Trigger the release pipeline manually to change the backend pool

**Package management**

**Azure artifacts** allows developers to publish code as packages so
that they can be used by other developers within organization

\- You have application that you have project in Visual Studio 2022
where you need to use functionality when it comes onto working with JSON
based data

\- Developer should look if code already exists that can help with JSON
instead creating code by themselves. There is package available in NuGet
package manager in VS which is called ***Newtonsoft.json*** that needs
to be installed as part of the project

\- It allows serialize and de-serialize JSON data instead writing code
from scratch by developer

\- When it comes to .NET, you have ***NuGet.org*** which has all of
these packages and Visual Studio going through NuGet to get all packages

\- Let consider some organization needs more control, they may need
private repository for the packages their developer create and separate
team to create packages for use of other developers within the
organization

\- For this purpose, you can use Azure Artifacts as own package
management solution in Azure DevOps

NuGet - .NET

npm - JavaScript

Maven - Java

PyPI Python package Index - Python

\- Develops can publish their packages and consume them in Azure
Artifacts

-Developers can additionally also consume their packages from public
feeds such as NuGet.org, npm etc

**Creating and publishing a package**

We build a package and publish it to Azure Artifact

\- Create new project with template using class library in C#

\- Rename the class library created as CoreFunctionality and create
simple method in the class

\- Create a new feed ***Create Feed*** in Azure Artifact to publish the
package so that other developers can connect the feed and consume the
packages. Specify the Name, Check the visibility for members, tick
Include packages from common public sources in Upstream sources,
Scope(project or organization)

\- Connect to the feed depending upon what language you are using to
either connect to the feed to publish or consume package, Check
***Connect to Feed***, select the language to connect to feed from your
machine specifying feed URL as source where it provides instruction to
set up your machine to connect the feed to publish or consume packages

Let consider you select NuGet to consume and publish packages

\- To restore or publish package to the feed, add package config
file(NuGet.config) to your project in same folder as yours .csproj or
.sln file

\- Unlike downloading package from public upstream source NuGet.org,
users have to authenticate when they connect to the feed in order to
consume package in the feed

\- You need to do 2 steps that shows when you select on ***Get the
tools*** in connect to feed section

Step 1: Download the latest NuGet - to publish or consume package

Step 2: Download and install the credential provider - If you don’t have
any edition of Visual Studio installed and you don’t need to
authenticate yourself every time, you can download credential provider
which will authenticate you first time to the feed and you don’t need to
enter credentials every time

\- Then download the latest NuGet, place NuGet executable file to folder
that contain source and project files of class library

\- Create new text file on your project in VS naming nuget.config and
copy xml content from ***Project setup*** section in ***Connect to
Feed***, save the file and build solution from VS

\- Go to properties section NuGet executable and check unblock security
feature that might be blocked to protect this computer

\- Navigate to the project directory from PowerShell as admin and run
nuget executable file with ***pack*** command to create a NuGet package
based on the specified nuspec or project file

./nuget.exe pack ./CoreServices.csproj

\- Thereafter shows that it created the package successfully e.g
CoreServices.1.0.0.nupkg

\- You can publish the package to the feed this command

nuget.exe push -Source “CoreServices” -ApiKey \<any string\>
\<packagepath\>

nuget.exe push -Source “CoreServices” -ApiKey Core
CoreServices.1.0.0.nupkg

\- Once run the command, it asks to sign in Azure DevOps account, it
shows as 'You package was pushed'. The package published you can see,
once refresh the feed after sign in to the account

**Consuming the package**

\- Create new project from ASP.NET Core Web App with new name

\- To consume the package created in the feed, go through Tools in VS \>
NuGet Package Manager\> Manage NuGet Packages for solution \> check
package source and go to settings(it will show nuget.org as default
package source)\> check + in package source to add new package source \>
select connect to feed with Visual Studio and copy name and source for
the feed \> place the name and source in package source and update, now
you can see your feed list in package sources

\- Select your package source which will need to authenticate to Azure
DevOps account. If you don't use Visual Studio, you have to download
credential provider

\- Browse the package you published, select ***consume the package***
and install on to the project. Then it will need to authenticate to
Azure DevOps account again and install the package

\- You can now make use to include core functionality method that
available in the package on to the project, ***consume package*** on VS
to check the functionality added into local host

**Azure Artifacts - Other aspects**

\- Feed is just a mechanism that allows you to store, manage and group
packages together

\- Normally the feeds are project-based. Here only people within the
project can access the feed

\- You can also create a public feed

\- The public feed allows you to share packages within anyone on the
internet such as nuget.org

*Requirements for public feeds*

\- They need to be created within public projects

\- They cannot have upstream sources

\- Public users cannot download universal packages

*Upstream sources*

-You can store and copy packages from different sources onto your feed

*Feed views*

\- Feed views helps to share certain packages as filtered way

\- The default views are @Local, @Prerelease, @Release

\- By default all packages are released to the @Local view

**Azure Artifacts - Upstream sources**

\- You can store packages from different sources onto your feed

\- The copy of the package from the upstream source will be stored in
the feed

\- When you create a feed, there is an option to check ‘Include packages
from common public sources’

\- You can see many upstream sources available when you go to settings
in feed

\- To set the private feed you created as default package source, go
through Tools in VS \> NuGet Package Manager\> Manage NuGet Packages for
solution \> check package source and go to settings\> uncheck nuget.org
and save

\- To install ***Newtonsoft.json***, get copy install command for
***Newtonsoft.json*** from nuget.org and go through Tools in VS \> NuGet
Package Manager\> Package Manager Console \> paste the command, run the
command that it will show the package is installed successfully after
authenticating through Azure DevOps account

\- Once you refresh the feed, you can see ***newtonsoft.json*** package
installed.

\- Ensure the package is downloaded onto feed to connect upstream source

**Lab - Azure pipeline - Package publish**

Where we take your project and publish it onto a feed using Azure
pipeline

\- Delete the package created and NuGet executable earlier from the
project

\- Change the version of package through properties of project \>
Package\> General\>Package version

\- Add version number to source file of method we created in the project

\- Create a git repository in Azure repos from the project and push it

\- Set up build choosing ASP.NET Core and configure YAML for building
code, creating a package(pack command with pack destination - artifact
staging directory), ***NuGet authenticate t***o authenticate to feed and
***NuGet push*** to push package to feed- publishVstsFeed: \<name of
project\>/\<name of feed\>, the build created

\# Build and test ASP.NET Core projects targeting the full .NET
Framework.

\# Add steps that publish symbols, save build artifacts, and more:

\#
<https://docs.microsoft.com/azure/devops/pipelines/languages/dotnet-core>

trigger:

\- main

pool:

vmImage: 'windows-latest'

variables:

solution: '\*\*/\*.sln'

buildPlatform: 'Any CPU'

buildConfiguration: 'Release'

steps:

\- task: UseDotNet@2

inputs:

packageType: 'sdk'

version: '6.x'

\- task: NuGetToolInstaller@1

\- task: NuGetCommand@2

inputs:

restoreSolution: '\$(solution)'

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: NuGetCommand@2

inputs:

command: pack

packagesToPack: '\*\*/\*.csproj'

versioningScheme: byEnvVar

versionEnvVar: Build.BuildId

packDestination: '\$(Build.ArtifactStagingDirectory)'

\- task: NuGetAuthenticate@0

displayName: 'NuGet Authenticate'

\- task: NuGetCommand@2

displayName: 'NuGet push'

inputs:

command: push

packagesToPush: '\$(Build.ArtifactStagingDirectory)\\.nupkg'

publishVstsFeed: 'AgileProject/CoreServices'

allowPackageConflicts: true

\- The build pipeline may fails as there is no necessary permission. In
that case go to feed settings, select *Project Collection Build
Service*, *AgileProjects Build Service* and assign contributor role,
then run the build the pipeline

\- Change the version of the package manually or add task to YAML file
to add the version of the package dynamically

**Pipeline reports**

\- Select any pipeline you created and check analytics pane where it
shows pipeline pass rate, test pass rate and pipeline duration

\- View full report shows duration takes by steps in the pipeline job,
you can optimize steps that took long duration to complete

\- In dashboard section, you can see widget and also you can add more
widget such as ***deployment status*** by choosing size(number of tiles
you use), build pipeline, linked release pipeline where it shows the
status of build pipeline and its linked release pipeline

**Flaky tests**

\- Flaky test present a barrier to finding real problems, since the
failures don’t relate to the changes being tested

\- Flaky test is a test that provides different outcomes, such as pass
or fail, even when there are no changes in the source code or execution
environment that actually cause particular pipeline to fail. Sometimes
pipeline fail even though it ideally pass

\- Sometimes build pipeline connects to external service which might be
down at that moment or unreachable. In that case, the pipeline might
fail even though there is no change on the source code

\- Flaky test is the option that allows you to automatically detect such
sort of failures

\- Project settings \> Test management \> you can flaky test detection
is on, detection type, all pipelines are enabled to flaky test
detection, enable flaky tests included in test pass percentage in Flaky
test option

**Azure App Configuration**

\- If you have configuration settings that need to be shared across
multiple Azure web apps instead defines configuration settings
separately in each Azure web app, you can use Azure app config service

\- If you want certain features to be rolled out to users, you can use
***feature flag*** to enable or disable the feature and also code the
use of feature flags

\- In Azure web app\> configuration \> you can define name value pairs
in terms of application settings and connection strings in the each
Azure web app separately

\- In Azur portal\> create App configuration \> resource group, name,
days to retain deleted store - 1, create

\- Create ***key value pair*** in ***configuration explorer*** that can
be used by Azure web app

\- Create new ***feature flag*** in ***feature manager***. You can
enable feature flag at point in time

**Using Selenium**

\- **Use selenium framework for user interface testing** for you web
application

\- As instance, you can test a keyword is coming as part of user
interface testing so that you can use Selenium

\- Create simple test project that use Selenium drivers, use template -
**MSTest Test project** in C#

\- Rename the UnitTest source as SimpleTest

\- Install Selenium web drivers in the project, go through Tools in VS
\> NuGet Package Manager\> Manage NuGet Packages for solution \> search
***Selenium.WebDriver*** and ***Selenium.WebDriver.ChromeDriver*** and
install the drivers in the project

\- Rename a TestMethod as TestURL which include new ChromeDriver,
navigate to web app URL(provide URL of Azure web app), check the title
of the home page

using OpenQA.Selenium;

using OpenQA.Selenium.Chrome;

namespace SeleniumTest

{

\[TestClass\]

public class SimpleTest

{

private IWebDriver test_driver;

\[TestMethod\]

public void TestURL()

{

test_driver = new ChromeDriver();

test_driver.Navigate().GoToUrl("https://docs.microsoft.com/en-us/learn/certifications/exams/az-400");

Assert.IsTrue(test_driver.Title.Contains("AZ-400")); - Get the title
from ***view page source*** by right clicking

//test_driver.Quit(); - close the browser after testing complete

}

}

}

\*\*The whole SeleniumTest project is available in course resources

\- ***Run all test*** from VS, it builds the project and run test. It
will open the app on the browser. The test result shows that test passes
as the web app contain the title

\- To close the app opened in browser, add quit method into source file

We can run Selenium test as part of Azure pipeline

\- Create git repository in Azure Repos for ***MSTest Test*** project ,
then create and push

\- Create build pipeline for the git repository pushed by adding build
and test steps to YAML file, save and run the build

\- Check the test result on build pipeline

trigger:

\- main

pool:

vmImage: 'windows-latest'

variables:

solution: '\*\*/\*.sln'

buildPlatform: 'Any CPU'

buildConfiguration: 'Release'

steps:

\- task: UseDotNet@2

displayName: Install .NET 6

inputs:

packageType: 'sdk'

version: 6.x

\- task: DotNetCoreCLI@2

displayName: Build

inputs:

command: build

projects: '\*\*/\*.csproj'

arguments: '--configuration \$(buildConfiguration)'

\- task: DotNetCoreCLI@2

inputs:

command: test

projects: '\*\*/seleniumtest.csproj'

arguments: '--configuration \$(buildConfiguration)'

**Azure Test Plans**

Testing - Planned manual testing, user acceptance testing, capture test
results

Feedback - You can also get stakeholder feedback with the help of Test
&feedback extension

Pipelines - There is integration with Azure Pipelines

Traceability- The test cases and suites can be linked to the user
stories features to provide end to end traceability

*Access levels*

Basic + Test Plans - Test planning (Create test plan and test suites,
manage test plan run settings, manage configuration), test execution(run
test on any platforms such Windows, Linux and Mac with test runner),
Perform exploratory testing with the Tests and feedback extension,
analyze and review tests

Basic - test execution(run test on any platforms such Windows, Linux and
Mac with test runner), Perform exploratory testing with the Tests and
feedback extension, analyze and review tests

Stakeholder- Perform exploratory testing with the Tests and feedback
extension

***Running tests***

***Test runners***

\- You can run the tests for your web and desktop applications

\- You can mark tests either passed or failed

\- The test outcomes can also gather results such as screen recordings
and screen captures

***Test & Feedback extension***

\- This is browser based extension that work with web application

\- You can get stakeholder feedback with the extension

\- The test outcomes can also gather results such as screen recordings
and screen captures

Test plans - This is used to group test suites and test cases

Test suite - This is used to group test cases into separate testing
scenarios

Test cases - This is used to define the actual steps required to test
the application

Shared steps - You can have shared steps that need to be shared across
test cases

**Subscribe to Test Plans trial**

\- You cannot do anything with test plans unless you at least get free
trial of subscription

\- Go organization settings\> Billing\> start free trial on Basic + Test
Plans

\- Once activate the free trial, change access level of users as Basic +
Test plans

**Creating Test cases**

\- In order to have end to end traceability, you can link test cases
with user stories in work items

\- Create a new test plan with appropriate name in a project

\- Create test suite which may be ***static, requirement based*** or
***query based***. Once you select a suite which creates a built-in
query. You can run query and find the user stories or work items

\- Select one of user stories and create test suite. Then create test
case with required steps in test suite

\- Then you can see the test cases are associated with user stories in
Azure boards

**Running test cases**

\- You can assign all test cases in test suites to test engineers so
that those test engineers must have necessary access level - Basic +
Test plans

-Select test suites in test plans \> Assign testers to run all tests\>
select testers (If you choose send email, tester can click the email and
start testing process)

-If the tester have access level Basic + Test plans

\- Select test points in Test plans and choose ***Run for web
application*** , this is going to run test runner on browser and mark
test points as pass or fail by adding comment, then login as tester and
testers can provide feedback based on what they see on test results

\- The test result will be propagated to all users in the project where
they can see the test result , you can ***view test results*** on ***run
explorer***

**Test and feedback extension**

\- This is to get feedback from your stakeholders. Let assume you
rollout new feature to application and need feedback from stakeholders

\- It doesn’t need Basic + Test plan license for stakeholder users

\- To get feedback, change the access level to stakeholder for user
which is free of charge\> go to user story for new feature \> ***Request
feedback*** from the user who has stakeholder access level, and send the
request feedback

\- To give feedback, stakeholder should install test and feedback
extension on his/her browser they use and also add ***Server URL*** -
<https://dev.azure.com/nibhathaka>, select the project in the
organization that needs feedback from, save

\- You can explore feedback( ***pending, completed, declined*** )\>
***view feedback*** \> ***provide feedback*** from browser extensions
itself. There are many options when you provide feedback from Edge
browser extension where you can

-When you start a session, you have these options ***capture browser
tab***(Browser, Screen, Application),***Add note***, ***Record
screen***, ***Create bug/Create task/Create test case***(with
stakeholder access level, you can’t create bug only basic + test plan
users can), ***View session timeline*** what you are doing, ***Explore
work items to link***, check session status, share screen capture. Then
you can stop the session

\- In Azure boards, you can see feedback response on boards as feedback
provided along with feedback comment, screen capture and also ***system
info*** of the browser the stakeholder used

**Develop security and compliance plan**

**Using variables**

Usage - Helps to define and reuse a value within the pipeline

Change - The value of the variable can change from run to run or from
job to job

Define - You can define the same variable in different places. The most
locally scoped variable will take effect

Expressions- You can also use variables within expressions

\- You can find variables in YAML file for build pipeline

\- To demonstrate, you can create repository as variable in Azure Repos
with README file. When you set up build for the repository, it gives you
option ***Starter pipeline*** and ***Existing Azure Pipeline YAML
file*** because the repository doesn’t have source code files with any
programming language

\- Add script to echo the variable

trigger:

\- main

pool:

vmImage: ubuntu-latest

variables:

databaseServerName: server4000

steps:

\- script: \|

echo \$(databaseServerName)

-Run the pipeline and check the console that return the output

\- Add bash script to change or set variable to existing variable

\- Add script to echo the variable

-Reference variable in different way

\- The step echo \${{ variable.databaseServerName }} will run at compile
time. But below script runs at run time

trigger:

\- main

pool:

vmImage: ubuntu-latest

variables:

databaseServerName: server4000

steps:

\- script: \|

echo \$(databaseServerName)

\- bash: echo "##vso\[task.setvariable
variable=databaseServerName\]server5000"

\- script: \|

echo \$(databaseServerName)

\- script: \|

echo \${{ variables.databaseServerName }}

**Defining variables in release pipeline**

\- You can specify variables that includes in pipeline tasks separately
as part of release pipeline where we refer ***Azure SQL Database
deployment, Azure Web App, Azure App Service Settings*** tasks in
release pipeline

\- In variable section, set name and value pair ***\$(sqlserverfqdn)***
abcs.database.windows.net unchecking settable at release time

\- set password as variable and change variable type to secret

\- Then you can run release pipeline and check the result

**Variable groups - YAML pipelines**

Storage - You can store values and secrets

Pipelines - You can access the values from the YAML pipeline

Usage - Variable groups can be used across multiple pipelines such as
build pipeline and release pipeline in a project

Azure CLI - You can also use the Azure CLI to work with variable group

\- You can create variable group in Azure DevOps,
Organization\>Project\> Pipeline\> Library\> + Variable group \> add
variable group name and name/value, add pipeline permission for what
YAML pipeline allows to use variable group

\- All classic pipelines can use variable group by default

\- To refer this variable group in build pipeline, add the following to
YAML file

trigger:

\- main

pool:

vmImage: ubuntu-latest

variables:

\- group: SharedVariables

steps:

\- script: \|

echo \$(databaseServerName)

**Variable groups - Classic pipeline**

\- Create a new variable group in Azure DevOps, Organization\>Project\>
Pipeline\> Library\> + Variable group \> add variable group name and
name/value

\- Navigate Variable groups in the release pipeline \> ***Link variable
group,*** choose ***SharedVariables*** \> Choose variable group scope as
Release or Stage \> Link \> Save

\- Where release pipeline imports variables from variable group linked

**Azure key vault**

\- Azure key vault is a Azure managed service where you can safely store
you secrets, certificates and encryption keys

\- Create key vault with name, Resource group, location, days to retain
deleted vaults as 7 days and with default configs

**Azure Key Vault - Pipeline**

\- Create secret that use at release pipeline by generating name and
value of secret manually so that you need key vault administrator role

\- In YAML pipeline, delete existing variables section in YAML file, add
***Azure Key vault*** task as 1st task in step to download Azure key
vault secrets. Add Azure subscription, key vault name, Secrets filter-
\*(To fetch any keys have in the vault), check if you need *Make secrets
available to whole job*. Then adding task make YAML syntax for adding
secrets to YAML file

trigger:

\- main

pool:

vmImage: ubuntu-latest

steps:

\- task: AzureKeyVault@2

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

KeyVaultName: 'appvault787878'

SecretsFilter: '\*'

RunAsPreJob: false

\- script: \|

echo \$(dbpassword)

\- Save and run pipeline while pipeline job runs, it shows '*This
pipeline needs permission to access a resource before this run can
continue* ‘ and permit

\- However, the pipeline will fail to run as error - '*Get secrets
failed. The user, group or application does not have secrets list
permission on key vault*'

\- To resolve this, we need to configure special type access permission
to key vault to allow security principal ID within the key vault that
authenticate Azure with Azure DevOps through service connection

\- To find the service principal, go project settings \>service
connection \> Azure subscription \> Manage app registration which will
navigate to is new application object registered in Entra ID when you
create service connection to Azure portal within the project in Azure
DevOps

\- In access configuration, you can add the service principal based on
the permission model you choose.

If it is Azure RBAC, assign ***Key vault administrator*** role to the
service principal.

If it is vault access policy(Legacy), Create access policy by adding
application ID of the service principal with secret permission- Get and
List

\- Run the pipeline again, it will run successfully and it will not show
the password in ***CmdLine*** step as it is secret type

\- To verify the secret echoing correct value of the secret, add code to
YAML file what it takes values of secret and put into txt file, copy
file in build artifact staging directory, then we can publish our build
artifact staging directory

\- Once the build pipeline runs complete, click the artifact produced in
the job which direct you to published artifact(secrets) \> TXT
file(dbpassword.txt) can be downloaded and you can see the plaintext
value of secret

trigger:

\- main

pool:

vmImage: ubuntu-latest

steps:

\- task: AzureKeyVault@2

inputs:

azureSubscription: 'Azure subscription 1
(6912d7a0-bc28-459a-9407-33bbba641c07)'

KeyVaultName: 'appvault787878'

SecretsFilter: '\*'

RunAsPreJob: false

\- script: \|

echo \$(dbpassword) \> dbpassword.txt

\- task: CopyFiles@2

inputs:

Contents: dbpassword.txt

targetFolder: '\$(Build.ArtifactStagingDirectory)'

\- task: PublishBuildArtifacts@1

inputs:

PathtoPublish: '\$(Build.ArtifactStagingDirectory)'

ArtifactName: 'secrets'

publishLocation: 'Container'

**Azure key vault - Variable group**

This covers how you can integrate secrets in Azure key vault with
variable group.

\- Variable group has an option to toggle ‘*Link secrets from an Azure
key vault as variable’*. If the variable group has variables, it prompts
a warning that to continue to link with Azure key vault, it would erase
all variables previously saved within this variable group.

\- If you create new variable group, integrate with Azure key vault
doesn’t prompt warning so that toggle\> select Azure subscription\>
select key vault name, Authorize\> +Add and choose secrets from the key
vault and save

\- Then you can specify variable group that import secret from key vault
with YAML or release pipelines

\- In this integration, variables are not synced from key vault
automatically. Adding new variable from vault is a manual task.

**Azure key vault - ARM Templates - Static reference**

This covers integration of Azure key vault with ARM template. We can
make integration in 2 ways.

1\. Static reference

2\. Dynamic reference

\- Instead hard coded password in sqldatabase-parameter.json add
reference for resource ID of key vault and secret name in Azure key
vault

{

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentParameters.json#>",

"contentVersion": "1.0.0.0",

"parameters": {

"SQLLogin": {

"value": "sqlusr"

},

"SQLPassword": {

"reference": {

"keyVault": {

"id":
"/subscriptions/6912d7a0-bc28-459a-9407-33bbba641c07/resourceGroups/template-grp/providers/Microsoft.KeyVault/vaults/keyvault67767"

},

"secretName": "dbpassword"

}

}

}

}

\- Before deploy the ARM template, check ‘*Azure Resource Manager for
template deployment’* in access policies in Azure key vault

\- Open Azure cloud shell with PowerShell, upload template files for
sqldatabse.json and sqldatabse-parameter.json

into Azure cloud shell

\- Check directory listing and run following command on cloud shell
where specify the resource group that include the key vault. You will
see output on cloud shell

az deployment group create - -resource-group Temp-grp - -template-file
sqldatabse.json - -parameters sqldatabse-parameter.json

\- Add firewall rule to connect sql server from you client IPV4 address

\- You can connect SQL database using password specified in Azure key
vault through query editor in SQL database

**Azure key vault - ARM Templates - Dynamic reference**

\- Previously, we referred the resource ID of key vault statically.
Instead we use dynamic reference for the key vault.

\- Further, parameters should not be in separate parameter file.
Instead, they should include in main template file where we have nested
template with sql username/password specified and parameters for the
values of sql username/password

\- We dynamically get the resource ID of key vault where we specify the
format of resource ID of key vault specifying the required values, also
use variable in the template to get subscription ID on the ARM template
is running in

\- Once main template file is ready, deploy the template from custom
template deployment in Azure

{

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"contentVersion": "1.0.0.0",

"parameters": {},

"functions": \[\],

"variables": {

"subscriptionId":"\[subscription().subscriptionId\]"

},

"resources": \[

{

"type": "Microsoft.Resources/deployments",

"apiVersion": "2020-10-01",

"name": "dbDeployment",

"properties": {

"mode": "Incremental",

"expressionEvaluationOptions": {

"scope": "inner"

},

"template": {

"\$schema":
"<https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#>",

"contentVersion": "1.0.0.0",

"parameters": {

"SQLLogin": {

"type": "string",

"metadata": {

"description": "The administrator user name for the Azure SQL Server"

}

},

"SQLPassword": {

"type": "secureString",

"metadata": {

"description": "The administrator password for the Azure SQL Server"

}

}

},

"resources": \[

{

"name": "sqlserver600505",

"type": "Microsoft.Sql/servers",

"apiVersion": "2021-08-01-preview",

"location": "\[resourceGroup().location\]",

"properties": {

"administratorLogin": "\[parameters('SQLLogin')\]",

"administratorLoginPassword": "\[parameters('SQLPassword')\]"

}

},

{

"name": "\[format('{0}/{1}', 'sqlserver600505', 'appdb')\]",

"type": "Microsoft.Sql/servers/databases",

"apiVersion": "2021-08-01-preview",

"location": "\[resourceGroup().location\]",

"dependsOn": \[

"\[resourceId('Microsoft.Sql/servers', 'sqlserver600505')\]"

\],

"sku": {

"name": "Basic",

"tier": "Basic"

},

"properties": {}

}

\],

"outputs": {}},

"parameters": {

"SQLLogin": {

"value": "sqlusr"

},

"SQLPassword": {

"reference": {

"keyVault": {

"id": "\[resourceId(variables('subscriptionId'), 'Temp-grp',
'Microsoft.KeyVault/vaults', 'valut1000')\]"

},

"secretName": "dbpassword"

}

}

}}}\]

}

\- Check ‘Set server firewall’ on top pane in SQL database and add
firewall rule to connect sql server from you client IPV4 address

\- You can connect sql database using password specified in Azure key
vault through query editor in sql database

**Using OWASP Tool - Build pipeline**

\- Open Web Application Security Project is a global community to
improve security of software.

\- There are top 10 security risk identified by OWASP.

1\. Broken access control

2\. Cryptographic failures

3\. Injection

4\. Insecure design

5\. Security misconfiguration

6\. Vulnerable and outdated components

7\. Identification and authentication failures

8\. Software and data integrity failures

9\. Security logging and monitoring failures

10\. Server-side request forgery(SSRF)

\- ***OWASP ZAP scanner*** is a tool that use to scan web application
and find risks that incorporate with based on OWASP guidelines

\- We can add task to scan the application from ZAP scanner as part of
release pipeline

\- The OWASP ZAP tool is available as docker image

\- To demonstrate ZAP scanner, we follows these steps in release
pipeline

- Create Azure web app and deploy app - Run a scan against the Azure Web
  App

- Create storage account using Azure CLI - file share to store report
  that is for scanned results

- Create container in ACI using Azure CLI - ZAP scanner docker container
  will actually run the scan against web application and results in
  container instance need to be persisted to store on file share in
  Azure storage account

- Download report using Azure CLI - download report from file share

- Convert report using PowerShell script - to convert report

- Publish test results - publish test results to pipeline

XSLT(Extensible Stylesheet Language Transformation) is a language for
transforming XML documents into other XML documents.

\- Clone an existing repository from Azure repos to VS 2022 and create
existing item for ***OWASPtoNunit.xslt*** file to create XML file for
test result of pipeline in the project. This file can be downloaded from
GitHub.

\- ***Commit and push*** the changes to git repository in Azure repos

\- Add ***PublishPipelineArtifact*** task into YAML pipeline to publish
XSLT file so that it is available in release pipeline

\- Commit the change to trigger YAML build pipeline

\- task: PublishPipelineArtifact@1

inputs:

targetPath: '\$(Build.SourcesDirectory)/owasp-app/OWASPToNUnit3.xslt'

artifactName: 'xslt-artifact'

**Using OWASP Tool - Release pipeline**

\- Make sure web application that connect to Azure SQL database is
functioning properly

1\. Create ***Azure CLI*** task to create storage account and file share
within storage account specifying Azure Resource Manager connection,
script type - PowerShell, script Location- Inline script, Inline
script - place the following Azure CLI commands

az storage account create -g template-grp -n owaspstore222000 -l
northeurope --sku Standard_LRS

az storage share create -n security --account-name owaspstore222000

2\. Create ***Azure CLI*** task to create container instance with
followings Azure CLI commands- image from DockerHub, public ip address,
port 8080, storage account name, azure storage account access key, azure
file share name, path of azure file share mount onto container, command
line to execute for scanning the web application using ZAP scanner.
Specify ARM connection, script type - PowerShell, script Location-
Inline script, Inline script - place the following Azure CLI commands

Provide name of storage account to mount file share with container
specify access key in storage account to authorize container to access
into storage account so that make command to list access keys in storage
account, get value of first access keys and put into txt file, get the
content of txt file and write the content with variable ***\$key***

Get the URL of the web app we test so that echo the URL, put into txt
file, get url from txt file and write the content with ***\$url***
variable, double code the ***\$url*** with ***\$comupterurl***. We have
another variable ***\$ZAP_COMMAND*** where zap-baseline application runs
within container passing the url that needs to be tested and generate
report in xml and html format

az storage account keys list -g template-grp --account-name
owaspstore222000 --query "\[0\].value" --output tsv \> temp.txt

\$content = Get-Content temp.txt -First 1

\$key = '"{0}"' -f \$content

Write-Output \$key

echo
"[https://newapp787878.azurewebsites.net](https://newapp787878.azurewebsites.net/)"\>
url.txt

\$url = Get-Content url.txt -First 1

\$completeurl = '"{0}"' -f \$url

\$ZAP_COMMAND="zap-baseline.py -t \$completeurl -x OWASP-ZAP-Report.xml
-r testreport.html"

az container create -g template-grp -n owasp --image
owasp/zap2docker-stable --ip-address public --ports 8080
--azure-file-volume-account-name owaspstore222000
--azure-file-volume-account-key \$key --azure-file-volume-share-name
security --azure-file-volume-mount-path "/zap/wrk" --command-line
\$ZAP_COMMAND --restart-policy Never

3\. Create ***Azure CLI*** task to download report from Azure file share
where we download report in xml format and store in the pipeline working
directory by accessing file share in storage account with access key
that get through txt file. Specify ARM connection, script type -
PowerShell, script Location- Inline script, Inline script - place the
following Azure CLI commands

Start-Sleep -Seconds 30 ; the release pipeline is failed because the
report generates from container takes time to be presence for
downloading. Hence it should make sleep for certain time before
proceeding downloads

az storage account keys list -g template-grp --account-name
owaspstore222000 --query "\[0\].value" --output tsv \> temp.txt

\$content = Get-Content temp.txt -First 1

\$key = '"{0}"' -f \$content

az storage file download --account-name owaspstore222000 --account-key
\$key -s security -p OWASP-ZAP-Report.xml --dest
%SYSTEM_DEFAULTWORKINGDIRECTORY%\OWASP-ZAP-Report.xml

4\. Create ***PowerShell*** task to convert the xml format report using
XSLT file stored in the project. Specify Display name, type-Inline,
Script - place the following PowerShell commands

Get the XSLT file path from linked artifact published from the build
pipeline and specify in \$XclPath. You can check the path by checking
file path in script path

\$XslPath =
"\$(\$Env:SYSTEM_DEFAULTWORKINGDIRECTORY)\\sqlapp-connection\xslt-artifact\OWASPToNUnit3.xslt"

\$XmlInputPath =
"\$(\$Env:SYSTEM_DEFAULTWORKINGDIRECTORY)\OWASP-ZAP-Report.xml"

\$XmlOutputPath =
"\$(\$Env:SYSTEM_DEFAULTWORKINGDIRECTORY)\Converted-OWASP-ZAP-Report.xml"

\$XslTransform = New-Object System.Xml.Xsl.XslCompiledTransform

\$XslTransform.Load(\$XslPath)

\$XslTransform.Transform(\$XmlInputPath, \$XmlOutputPath)

5\. Add ***Publish Test Results*** task by specifying Display name, test
result format- NUnit, Test results files - get name of converted file
from variable ***\$XmlOutputPath*** that generated from last PowerShell
script

Then run the release pipeline. Once release pipeline is success, you can
see test results of OWASP ZAP scanner on Tests pane on release pipeline.

The container instance may fail after scanning the ZAP scanner tool.

**Review of service connections**

\- Azure DevOps use service connection when Azure DevOps uses to connect
external service such as Azure subscription, GitHub, Azure Kubernetes
Service (outgoing connection)

\- Go project settings \> Service connections, to create service
connection that can use within Pipeline securely without entering
credentials each time to connect instead of embedding credentials to
connect external service

**Review of Personal Access Token**

\- Azure DevOps generates PAT when some external service needs to
authenticate onto Azure DevOps( incoming connection)

\- User settings\> Personal access token\> New token \> Specify name,
organization, expiration, scopes(full access or custom defined), custom
defined option have work items, code, build, release, test management,
packaging

\- Generally PATs are generated for ***self-hosted agent*** that needs
to be part of agent pool, VMs that needs be part of ***deployment
group***

**Secure files**

\- You can upload your secure files as part of variable groups

\- With this you can store secure files such as your certificates or SSH
keys that can be used across the pipeline

**GitHub code scanning**

\- One of the security features that available in GitHub

\- GitHub can scan your code for any sort of vulnerabilities

\- For your code in GitHub, go to actions\> workflow\> Search for
Security and CodeQL Analysis

\- This will add a CodeQL based workflow file to your code. You can do a
commit of this new file. This will the trigger a job.

\- It will show you any vulnerabilities and let you know if the code is
fine

**Implement an instrumentation strategy**

**Azure monitor service**

\- In Monitor service, you can enable metrics, logs, alerts, service
health, activity logs on resources in resource group, use ***save to
dashboard*** to maintain your own dashboard to monitor

\- If you deploy resource using ARM template and if it fails, there are
event occurs that you can see on Azure monitor logs with reason in
message

**Azure monitor- Setting up alerts - Static thresholds**

\- You can set up alert rule to trigger alert to IT admin based on
condition such as certain threshold value on CPU reaches for a VM, HTTP
response errors that receive to users for Azure web app

\- When you create alert rule, you need to specify the following.

scope : select the resource you want to monitor in subscription

condition :

signal type- If you choose metrics of percentage CPU (metrics, log,
activity log, resource health)

alert logic(static, dynamic)

define the threshold with aggregation type(average)

***frequency of evaluation***- how frequent rule checks the alert logic
on threshold values

***aggregation granularity period***- how far back aggregation of the
metric values evaluate each time to generates alert

Ex: Consider aggregation granularity period is 15 minutes, the metrics
should be evaluated in its frequency whether metrics (CPU percentage)
exceeds threshold value for last 15 minutes based on aggregation type

Actions: create action group specifying name of action group,
notification- notification type(Email/SMS message/Push/Voice), action -
action type( automation runbook, Azure function, event hub, logic app,
ITSM, Secure webhook, webhook)

Details: severity, alert name

**Azure monitor - Dynamic thresholds**

\- Azure monitor uses machine learning to check the historical behavior
of metrics

\- Based on historical data, it can then identify patterns and anomalies
that could indicate possible issues

\- ***Threshold Sensitivity*** in alert logic is a feature you can
define in dynamic thresholds where it monitors historical ideal patterns
of metrics and identify deviation against the pattern based on the
historical data that extracted

High - the alert rule will be triggered even for the small deviation

Medium - you have more balanced thresholds and fewer alerts will be
generated

Low - alerts will only be triggered on large deviations

\- Define evaluation criteria on threshold sensitivity where advanced
settings provides such as ***number of violations*** to trigger the
alert, evaluation period, ignore data before specific time period

**Log analytics workspace**

\- A central repository to collect logs and store for resources such as
Azure VM, on-premise servers, Azure SQL database audit information

\- For some resources, you can directly connect from Log analytics
workspace and also other resources, you can use ***diagnostic setting***
to send data to log analytics workspace

\- ***Kusto Query Language(KQL)*** is used to query the data in log
analytics workspace

-You can have solutions in-built on top Log Analytics Workspace that can
work with that data and give visualization

\- Create a log analytics workspace specifying name, resource group and
location, create

\- To connect from log analytics workspace itself\> select virtual
machine \> select the VM \> Select ***connect*** where it installs the
***Log analytics agent*** as an extension in the VM through which log
analytics agent connect to log analytics workspace and send the data
accordingly

\- You should decide type of data that needs to be collected to log
analytics workspace. In log analytics workspace, agents management \>
create ***data collection rule***\> Rule name, region, platform
type(windows, Linux, custom)\> resource - select the VM \> Collect and
deliver\> Data source, data source type( performance counters, windows
event logs- choose what events you need to collect), Destination, add
log analytics workspace\> create

\- To connect log analytics workspace from ***diagnostic settings*** \>
In Azure SQL database \> add diagnostic settings\> name of diagnostic
settings \> check all logs and send to Log Analytics Workspace, it takes
half an hour to appear collected logs in Log Analytics Workspace

\- Go to logs in log analytics workspace \> filter resource type \>
query the logs

**Service Map solution**

Discovery - Helps to discover application components on Windows and
Linux systems

Information - You can see information such as connections between
servers, latency for connections

Log analytics- The machine need to connect to log analytics workspace

Agent - The machine also need to have the ***Dependency agent***
installed

\- To use service map, first the VM need to connect log analytics
workspace and install Dependency agent as an extension. We can install
the Dependency agent manually or using ARM template. You can see
***DAExtension*** in Extension + application section in the VM

\- Once the agent is installed, go to workspace in log analytics
workspace \> workspace summary\> add ***Service Map*** from marketplace
and create \> choose subscription, resource group, Azure log analytics
workspace, create

\- It takes certain time to collect data to ServiceMap from VM. Then
ServiceMap shows visual interface the number of clients who connect to
the VM with their IP addresses, services/processes/ports running on the
VM

**Virtual machine scale sets extension**

\- In virtual machine scale sets, we can set up ***custom autoscale***
in scaling. By default it has ***Auto created scale condition***

-Additionally you can configure more auto created scale condition with
scale mode(scales based on a metric, scale to specific instance count),
Add rules, instance limit, schedule to start and end date. Once the
condition meets, auto scaling rule create new instance in virtual
machine scale sets

\- In scaling, we can send notification through email or webhook, go to
Notify and put email ID

\- In scaling, Go to diagnostic settings\> add diagnostic setting\> name
for diagnostic settings \> Categories - ***Autoscale Scale Actions***\>
Destination details - check Send to log analytics workspace and select
the workspace created

\- If the scale condition meets, you can see additional VM instance
created, email triggered and logs available to query in the workspace,
you can query table ***AutoscaleScaleActionsLog***

**Application Insights**

Monitoring - This provides the feature of application performance
management and monitoring of live web applications

Aspects - You can see aspects such as detecting performance issues or
any other issues

Support - There is support for .NET, Node.js, Java and Python

Applications - This works for applications hosted in Azure, on-premises
environments or other cloud platforms

Integration - It has integration with the Visual Studio IDE

Users - You can also see how users interact with your application

How does it work;

\- You can install a small ***instrumentation package(SDK)*** for your
application or use ***Application Insights agent***

\- You can instrument web application, background components and
JavaScript in web pages

\- The telemetry data sent by Application Insights has very little
impact on the overall performance of your application

**Use of Application Insights**

\- Create Azure web app by specifying name, publish, runtime stack and
enable Application Insights, create new Application Insights, it gets
workspace automatically and its region.

\- Go to Azure web app\> Instrument your application, .NET Core \>
collection level-recommended

\- Create a project in Visual Studio and make a change onto index.cshtml
page

\- To integrate the project with Azure application insights, Choose
***configure application insights***\> configure dependency- Azure
Application Insights\> Choose Azure application insight instance \> it
automatically configure connection string \> Finish. It installs NuGet
packages for instrumenting application insights on application itself

\- Publish the project by creating publish profile to Azure web app

\- Go to application insight \> Live metrics, streaming connects to the
application. When you navigate different pages on web application, you
can see live metrics and telemetry such as Incoming requests- request
rate, request duration, request failure rate, Outgoing requests-
dependency call rate, dependency call duration, dependency call rate

**Application insight - Availability test**

\- To verify from application insights whether the web app is always
accessible from different locations, we can create availability test
within application insights

\- In application insight\> Availability \> Add standard test\> Provide
a test name, URL of web app that need to test, check ***parse dependent
request*** if your web application has images, JavaScript and whether
load is expect, choose test frequency, choose test location- choose
regions you want to check from, standard test info- HTTP request
verb-GET, success criteria(HTTP response: 200), enabled alerts

\- After 15-20 min, you can test result of availability test with
duration, availability, details of end to end transactions

**Application Insights- Other features**

These features are from exam perspectives.

Users- you can see how many people have used your application and its
features

Session - You can see sessions of user activity. This includes certain
pages and features of the application

Events- This gives a view of how often certain pages and features have
been used in the application

Funnels- you can have multiple stages like a pipeline and then you can
see how users are progressing through the application as an entire
process

Cohorts- This is set of users, sessions, events or operations that have
something in common. It helps to analyze a particular set of users or
events.

Impact - you can see how load times and other aspects of your
application impact ten conversion rate for your application

Retention - you can analyze how many users return back to the
application

User flows - it provides answer for following use cases

\- What do users click on a page within the application

\- Where are places within the application that uses churn the most from
the site

\- Are there places in the application where the users repeat the same
action over and over again

Performance- GET request operations with average duration and count

***Smart detection - Failure anomalies***

This feature allows to alert automatically in real-time time if the web
app experience an abnormal rise in the rate of failed requests.

If you direct through Azure Monitor\> Alerts\> action group\>
application insight smart detection- there is an action group from this
name that created from application insight itself automatically. You can
edit to add own notification and action apart from pre-defined
notification and actions

\- When we create application insight along with web app, it creates a
log analytics workspace to store logs and alert that are generated by
application insights as naming DefaultWorkspace

\- You can create application insight separately and associate it to
existing workspace

\- Application insights visualize the data that store in log analytics
workspace

**Azure container instances probes**

\- You can create container instance using YAML file with the use of
container group

\- In YAML deployment, you can specify ***liveness probe***,
periodSeconds to check should be in place

\- What liveness probe does is that the container instance will restart
the container if the container doesn’t work properly with some error for
some reason

\- When the container depends upon a database, we use ***readiness
probe*** that has command to check availability of data in database in
order to start application container

**Azure DevOps notification**

\- There are many built in notifications for each services in Azure
DevOps

\- You can customize notification by adding new subscription with
categories and its template

\- User settings\> notification \> add subscription

-There are pre-defined notification for Build, Code

<img src="./images/4ac24a2f6525fab18f81de0caa1b6a384852940a.png"
style="width:9.625in;height:5.41667in" />

**IT Service Management Connector**

\- Events and incidents occur on Azure service where Azure monitor need
to integrate with service management tools such as ServiceNow, BMC

\- Using IT Service Management Connector, it triggers incident, request
your ITSM tool whenever Azure Monitor creates alert or event
