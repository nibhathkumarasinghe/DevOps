**Azure DevOps Note**

When hiring, remember that not all DevOps Engineers are the same. 

Some are strong in CI/CD.  

Some are skilled in scripting.  

Some are specialists in security.  

Some are great with containers.  

Some are proficient in IaC tools.  

Some are experts in Kubernetes.  

Some are pros at cost optimization.  

Some are specialized in networking.  

Some are focused on cloud platforms.  

Some are excellent at disaster recovery.  

Some are passionate about observability.  

Some are great with hybrid environments.  

Some are experienced in performance optimization. 

Most can handle some of these or a mix of them. 

But no DevOps Engineer should be expected to master or handle all of
them.

Be clear about what you need and hire a DevOps Engineer who fits those
specific needs - not EVERY SINGLE THING.

Thoughts ?

**Introduction**

**Design and implement build pipeline**

Continuous Integration - Automatically building and testing code every
time a team member commits code changes to version control

Build and Publish process - The build tool builds the
project/dependencies to a set of binaries and publish to target location
that has required runtime

Azure Pipeline - Use to build and test code through continuous
integration and continuous delivery/Deployment. Create
azure-piplelines.yml file that is versioning

Creating pipelines - select remote repository\> select code in
repository \>select underlying programming language \> change the YAML
definition adding tasks in step( initializes the job, download the
required tasks, checkout code from repository, build the code using the
task )

Terminology in Azure build pipeline - trigger, pool, Variables,
PackageInstallation, Restoresolution, Build, Publish,
PublishPipelineArtifact

Microsoft hosted agent - agent using VMimage(Windows/Linux) with
language and runtime, package management, environment variables, fresh
VM for each pipeline job

Self-hosted agent - when you need to store build of source code project
on machine, custom software installed/third party components for build,
store builds in another location

Deploying self-hosted agent - Create a new VM, Install git and required
runtime for app(.NET SDK)

Registering the self-hosted agent with Azure DevOps - generate a
Personal Access Token, Download the agent to new VM from agent pool,
Create new directory and extract agent file, Navigate to the directory,
run ./config.cmd on Powershell, Register the agent with Azure DevOps
server(Server URL,PAT,agentpool,agentname,work folder to store build)

Exploring the work folder - Source code stores in
c:\work\1\s(Build.SourcesDirectory), add publish task to get the build
code from c:\work\1\a(Build.ArtifactStagingDirectory)

Security at every stage - Threat modeling (during design/ planning
phase), Static code analysis(during CI phase), Dynamic code
analysis(during runtime), Penetration testing(after CI/CD processes)

Mend Bolt tool - open source software security and compliance management
tool to detect security and vulnerabilities, open source libraries with
outdated licenses, to identify license requirement, potential
vulnerabilities and outdated libraries

Using the Mend Bold tool - Integrate Azure DevOps account with Entra ID,
Install Mend Bolt extension in Azure DevOps organization, Activate Mend
Bolt extension, add Mend Bolt task to pipeline and run build pipeline,
generates open source risk report with security vulnerabilities, license
risks, inventory in Mend Bolt section in the pipeline

Adding and running unit test - add xUnit Test project within main
project, add a test task into pipeline, show test result on Test pane in
the pipeline

Code coverage - Add new method based on function class into test
project, run all test and push the code to Azure Repos, Install package
on test project and push the code to Azure Repos, add test task for code
coverage tool(Cobertura or JaCoCo), Add task to publish code coverage
result to pipeline

GitHub repository - Azure pipeline authorize to GitHub using GitHub app,
OAuth and Personal Access Token

GitHub status badge - to reflect status of the pipeline to GitHub, paste
sample markdown into readme file in the GitHub repository, uncheck
disable anonymous access to badges at organizations and project settings
level

Azure pipeline Classic Editor - GUI version for Azure pipeline apart
from YAML pipeline, select other Git to get classic editor, create
generic Git service connection to other git repository using PAT
generated from other end

SonarCloud - improve source code quality and security, to integrate
SonarCloud with Azure DevOps(1.Create a project and organization in
SonarCloud 2.Generate SonarCloud token 3.Create new service connection
to SonarCloud),Install SonarCloud extension Azure DevOps organization,
Add tasks create tasks prepare analysis configuration, run code
analysis, publish quality gate result into pipeline, shows result of
code quality analysis in SonarCloud

Parallel jobs - MS hosted CI/CD - 1 parallel job, Self hosted CI/CD - 1
parallel job, purchase license for multiple parallel jobs

Pipeline caching - to reduce the build time spends for the pipeline
jobs, some projects need multiple packages to be downloaded from
internet, cache packages using cache task to the pipeline

Azure pipeline integration with Microsoft Teams - Add Azure pipeline app
in Teams, @azure pipeline subscribe \[project URL\] \| \[pipeline URL\]

Using GitHub actions - to trigger Azure pipeline using GitHub
workflow, 1. Create workflow.yml in the GitHub repository 2. Generate
PAT from Azure DevOps for GitHub actions 3.Create a New organization
secret for variable -AZURE_DEVOPS_TOKEN by specifying PAT 4. Commit all
and push change to GitHub, action pane in GitHub how pipeline runs

Jenkins - open source CI/CD tool, Jenkins installation on Linux VM(1.
Install Jenkins 2. Start Jenkins 3. Unlock Jenkins with admin password
4. Install required plugins)

Creating a build pipeline in Jenkins - Install git and required runtime,
Elevate permission on working directory that store build and projects,
Create a build pipeline as freestyle project

Jenkins Integration with Azure Repos - Create a build pipeline as
freestyle project repository from Azure Repos, create new service hook
subscription in project settings in Azure DevOps to trigger the build
process in Jenkins automatically when commit changes in Azure Repos

Managing agents - Reader, Service account, Administrator

**Design and implement release pipelines**

Understand deployment - After CI process, the app needs to deploy to
development, test, staging, production environment as part of CD process

Azure Web App - Manual Deployment - Create Azure Web App, Publish the
code using publish profiles

Azure Web App - Release pipeline - Add PublishPipelineArtifact task in
build pipeline, Add Azure Web App Deploy task in agent job, Enable
continuous deployment trigger

Multiple stages in the pipeline - to maintain multiple environments

Approvals and gates - Approvals are manual approaches whereas gates are
automate approaches

Release pipeline - Approvals - Enable pre and post deployment condition
with manual approval over email or ADO portal itself

Azure pipeline- Gates - post-deployment conditions : Query work
items(shared query on Azure Boards that is not closed), Query Azure
Monitor alerts(alert rule with condition of average memory of Azure web
app), Check Azure policy compliance (Azure policy definition and
assignment for not allowed resource types)

Azure release - Manual Intervention - manual intervention task in
agentless job to resume/reject the stage manually

Deployment Groups - to deploy application to multiple machines at a
time,(1.create VMs installing IIS and ASP.NET Core 6, 2.Create
deployment group, 3. Copy the registration script, 4. Run the script on
Windows PowerShell at target VMs), VMs are registered shows as targets,
add a deployment group job including IIS web app manage and IIS web app
deploy tasks in release pipeline

Azure SQL database - Manual Deployment - Create a Azure SQL database in
SQL server, create a table using query editor, Specify database server
name/username/password/database name in the productservice.cs file, Run
the app on Visual Studio to connect Azure SQL database from IDE

Azure Web App - Azure SQL database - Manual Deployment - Create Azure
Web app in Azure portal, Create build pipeline with publish pipeline
artifact, Create release pipeline with Azure Web app task, Trigger the
build pipeline, Azure web app connects through static string from
published code itself to Azure SQL database

SQL Database table using Azure pipelines - Create release pipeline with
Azure SQL Database deployment task to create a table using inline
script, Azure Web App task to download web app artifact and deploy onto
Azure Web App

Azure Web App - Connection String using Azure pipelines - Create
connection string in Azure Web App with ADO.NET value to connect to
Azure SQL database, Specify GetConnectionString details to fetch
connection sting onto the code and publish the code to Azure Repos,
Create Azure App Service Settings task in the release pipeline after
Azure Web app task

Release pipeline- Associate work items - Edit release pipeline \>
Options \> integration \> Check 'to report deployment status to work'
with desired stage , commit a change by linking a work items using Works
items to link

Containers - Building a Docker image - Manual approach - Install Docker
on an Ubuntu VM, Publish the project to local directory, Copy the
published code onto Ubuntu VM, Create Dockerfile to make docker image,
Move Dockerfile into the directory that has published code with DLL, Run
docker build command

Deploying a container - Manual approach - Create a container registry on
Azure, Install Azure CLI tool on VM, Log into Azure container registry,
Tag the docker image built, Push the image to the Azure Container
Registry, Create Azure Container Instance with image source(ACR)

Azure pipeline - Azure container registry - Add the Dockerfile into
project folder, Create git repository in Azure Repos and push the
project, Set up build pipeline with option Build and push an image to
ACR, Provide Azure credentials to authorize with service connection to
ACR, Create build pipeline with stages and tasks - trigger, resources,
variables, Build stage(pool, UseDotNet task- install SDK, DotNetCoreCLI
task- build, DotNetCoreCLI task- publish, Docker task- buildAndPush
image)

Azure pipelines - Azure Container Registry- Debugging - Docker task may
still take the source code instead of the build, add PowerShell task
after .NET Core publish task into YAML file which shows files with size,
name, permission level

Azure Container Instance - Release pipeline - Create agent job with
Azure CLI task that create ACI with image pushed

Deployment to Azure Kubernetes Service - Manual approach - Create Azure
Kubernetes Service integrating ACR, Create Deployment and service
manifest files to deploy on AKS, Create deployment on workload, Create
service on Services and ingresses, Access external IP of service once
deployment is ready state

YAML Pipelines - Deployment to Azure Kubernetes Service - Create service
connection to AKS cluster, Add deployment and service manifest files/
Dockerfile into project folder, Create git repository in Azure Repos and
push the project(Stop the trigger), Set up build pipeline with option
Build and push an image to ACR, Provide Azure credentials to authorize
with service connection to ACR, Create build pipeline with stages and
tasks - trigger, resources, variables, Build stage(pool, UseDotNet task-
install SDK, DotNetCoreCLI task- build, DotNetCoreCLI task- publish,
Docker task- buildAndPush image, Add a Deploy to Kubernetes task - to
deploy deployment/service manifest files)

Release pipeline- Azure Kubernetes Service - Create service connection
to AKS cluster, Add deployment and service manifest files/ Dockerfile
into project folder, Create git repository in Azure Repos and push the
project(Stop the trigger), Set up build pipeline with option Build and
push an image to ACR, Provide Azure credentials to authorize with
service connection to ACR, Create build pipeline with stages and tasks -
trigger, reseources, variables, Build stage(pool, UseDotNet task-
install SDK, DotNetCoreCLI task- build, DotNetCoreCLI task- publish,
Docker task- buildAndPush image, Add PublishPipelineArtifact task - To
publish build artfact to release pipeline), Create release pipeline
specifying published artifact(Add a Deploy to Kubernetes task - to
deploy deployment manifest file, Add a Deploy to Kubernetes task - to
deploy service manifest file)

Publish artifacts - publish all source files from build to release
pipeline using PublishPipelineArrifact task

Multi-stage builds - to perform build and publish with the help of
Dockerfile, Store the Dockerfile in project folder, Create git
repository in Azure Repos and push the project(Stop the trigger), Set up
build pipeline with option Build and push an image to ACR, Provide Azure
credentials to authorize with service connection to ACR, Create build
pipeline with stages and tasks - trigger, reseources, variables, Build
stage(pool, Docker task- buildAndPush image, Add PublishPipelineArtifact
task - To publish build artfact to release pipeline) \*\*It doesn't need
task to install runtime, build and publish in the build pipeline

Container jobs - To avoid conflict with different packages in
self-hosted agent, containers have their own tools and save cost for the
build

Working with container job - Create git repository in Azure Repos and
push the project(Stop the trigger), Set up build pipeline with option
Build and push an image to ACR, Provide Azure credentials to authorize
with service connection to ACR, Create build pipeline with stages and
tasks - trigger, reseources, variables, Build stage\[pool(vmImage,
container base image), DotNetCoreCLI task- build, DotNetCoreCLI task-
publish, publish task- to publish Deploy stage\], Deploy
stage\[pool(vmImage), download task - to download published build,
Docker task- buildAndPush image to ACR, Add a Deploy to Kubernetes
task - to deploy deployment/service manifest files\]

Technical Debt - Sonarcloud helps to maintain the stability and quality
of the application code, Technical Debt Ratio: Remediation cost /
Development cost, To reduce the accumulated technical debt: reducing
code coupling and dependency cycles, Reduce the code complexity

When there are multiple builds - Use deployment queue settings with
options deploy all in sequence and deploy latest and cancel the others,
specify number of parallel deployment

**Design and Implement Infrastructure as Code**

Managing infrastructure
