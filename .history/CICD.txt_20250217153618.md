# Importance of Continuous Integration

 Improves the quality : By running multiple tests and analysing various static code.

 Increase Productivity : Automating build of code saves a lot of time, thereby increasing Productivity
 
 Reduces Risk : Eliminate the risk of potential humour errors by automating tests.

## Introduction to Jenkins 

 ## Features of Jenkins

 1. Easy Installation Process.
 
 2. Provides advanced security.

 3. Optimized Performance.

 4. Upgrades are easily available.

 5. Light weight containers support.

 6. Distributed Team Management.

## What is Continuous Integration

It is the process of automating the building & testing of code, each time one of team membercommit changes to version control.

CI- Continuous Integration

CD-Continuous Delivery/deployment &  Continuous Delivery is also knows as Release.

## Popular Continuous Integration Tools:

    --> GitLab

    --> Codeship

    --> Bamboo

    --> Jenkins

    --> Teamcity

    --> Travis CI

--> From AWS cloud if we wanted to perform CI/CD there are various services like code commit,code deploy,code guru,code build and code pipeline.

--> In Azure cloud we have Azure devops,azure boards,azure repos,azure pipelines,azure test plans & azure artifacts.

## What is jenkins

A continuous Integration server/automation server which manages & control processes such as plan,code,build,test,deploy operate & monitor devops environment.

## Why Jenkins is so Popular 

     --> Open source

     --> Good plugin support
      
     --> Good community support

     --> Fast & Reliable

     --> Good OS support 

     --> Scripted Builds

## Following are the Topics covered in this Module:

* Jenkins Architecture

* Plugin Management in Jenkins

* Jenkins security Management

* Notification in Jenkins

* Jenkins Master slave architecture

* Jenkins Delivery Pipeline

* Jenkins Declarative Pipeline

## Jenkins Architecture: source code Management

  Git --> Jenkins
             |--> Build+unitTest --> Function Test --> Deploy |--> Test Environment 
                                                                                    |
                                                                                    |--> Release Environment
                                                                                    |
                                                                                    |--> Production Environment

## Purpose of Plugins 

To have Extra fuctionality we will going for Plugins

## Plugins Management in Jenkins

  Tabs ----> |-------------> Update -------> Shows Updates to plugins already installed
                | 
                |-------------> Available --------> Shows Plugins that are available for installation
                |
                |-------------> Installed ----------> Displays Plugins installed that have no updates
                | 
                |--------------> Advanced ---------> Lists configuration of HTTP proxy, allows manual upload of plugin URL of plugin site

In Real time we cannot install the plugins as simple as that reason being their might be challenges with proxy settings as well as vpn(virtual private cloud/Networking) Inorder to avoid we should configure HTTP proxy in jenkins plugin of advance Tab.

## How to install Jenkins on Windows

## Different ways of Installation
               
     ---> Using Docker

     ---> Using Kubernetes

     ---> Using Linux

     ---> Using war file as well as offline     installations

     ---> Using Macos

     ---> Using windows

     ---> Using servlet containers              
             
## Prerequisites:

 Minimum Hardware Requirements
 
    --> 256 MB of Ram

    --> 1GB of drive space

Recommended Hardware Configuration for a small team

    --> 4GB of RAM

    --> 50GB of drive space

Jenkins tools is developed on Java code.

## Prerequisites:

--> system running windows 10

--> The Latest copy of Java Development Kit / Java Runtime Environment installed

--> Browse to downloads page of jenkins.Under the downloading jenkins section is a list of installers for the long term support(LTS) version of jenkins.Click the windows link to begin the download.

-->URL- Jenkins.io/download/ --> Download jenkins 2.4/9.3 LTS

--> Once ou click on windows text under download jenkins it will open new tab saying thankyou for  downloading.

--> Once after download need to go to download folder double click on jenkins file which is of type windows installer package.

--> The setup wizard starts clicks next to procees.

--> Select the install destination folder & click next to continue.

--> Under the run service as a local / domain user option, enter the domain username & password for the user account you want to run jenkins with clicktest credentials to verify the login data, then click next to proceed.

--> Select first option which is run service as Local system.

--> Enter the port number, you want jenkins to run on. Click test port to check if the selected port is available, then click next to continue default port number of jenkins is 8080.

--> Select the directory where java is installed on your system & click next to proceed.

--> Select the features you want to install with jenkins & click next to continue.

--> Click install to start installation Process.

## How to configure jenkins

--> After completing the installation process, you to unblock jenkins before you can customize & start using it.(Localhost:8080)

--> In your web browser,navigate to the port number (default port number) you selected during the installation using the following address
  
syntax: http://localhost:[port number]

           http://localhost:8080

           127.0.0.1:8080

--> Navigate to the location on your system specified by the unlock jenkins page.

--> Please copy the password from Location 

    c:\programdata\Jenkins\.Jenkins\secrets\initialadminpassword

--> where initial admin password is a file inorder to read to the data of the file use cat 

     c:\programdata\Jenkins\.Jenkins\secrets\initialadminpassword

--> Copy the password from the InitialAdminPassword file

--> Paste the Password in the Administrator password field on the unblock jenkins page & click continue to Proceed.

## Customize Jenkins

--> Click install suggested plugins button to have jenkins automatically install the most frequently used plugins.

--> After jenkins finishes installing the plugins, entered the required information on the admin user page. Click save & continue to Proceed.

--> On the instance configuration page, confirm the port number you want jenkins to use & click save & finish.

## How to stop jenkins server on windows

 --> Go to services of windows & search for jenkins once you click on this will be seeing left side start & stop

## How to Restart the Jenkins


## Safe Restart

--> Go to URL of jenkins & http://localhost:8080/ safe restart

--> Jenkins will try to pause jobs and restart once all running jobs are either finished or paused.

## Jenkins Restarting Banner

  ----> This will be displayed on most jenkins pages,ou can use it to let users knows what is happening. A default message will be added if you don't supply one.


## Plugin Installation

--> There are two ways to install the plugins
   
    1. Automatically

    2. Manually

## Automaticallty    

   --> once you login to jenkins GUI left side you will see the option of manage jenkins click on manage jenkins in first tab there is a system configuration under that you can see plugins.

   --> Now click on plugin then go to available plugins search for the plugin which is required then select the plugin under the list once you select the plugin install button will be highlighted then click on install button.

## Manually

  --> Under plugins tab go for available plugins & search for the plugin click on the plugin which is required. Once you click on the plugin new tab will be open then click on releases under releases you will see the various versions of plugins go for the plugin which is required specific version then click on direct space link. Yow will see installations option.

  --> Once you click on direct link plugin will get downloaded to local machine/local system.

  --> when we downloaded plugin in manual way again we need to deploy to jenkins.In jenkins GUI plugins tab click on advanced settings there you can search for the choose file button to upload whcih is downloaded to loacl machine or local system 

## Plugins

  --> Plugins can add, remove, disable/enable plugins that can extend the functionality of jenkins.

  --> when we install plugin in automatic way plugins extension is JPI(Jenkin Plugin)

  --> when we install plugin in manual way the plugins extension is HPI(Hudson Plugin)

## How to uninstall the Plugins

 Go to manage jenkins --> plugins --> install plugins search plugin name which we wanted to uninstall.

 --> select the plugin & then uninstall button will be highlighted once clicked on uninstall, plugin will get uninstalled.

## How to update the Plugin

Go to Manage jenkins --> plugins --> updates

--> slect the plugin then update button will be highlighted once clicked on update, plugin will get updated.

--> In real time we should not update the plugins directly reason being there may be challenges will be encountered. It will be recommended to update the plugin in our local machines where other team members will not get affected if anything goes wrong.

## How to create the users

--> Manage jenkins-->security-->users(create/delete/modify users that can log in to this jenkins) click on users we will see the option users.Create user,username,password,confirm password,Fullname & email address then click on create user.

## How to give permissions to the users

--> Manage jenkins --> security(secure jenkins,define who is allowed to access/use the system) then will see authorization under that you will be seeing.Add user button click on add user it will show user id & click ok button.You should see user is added then give the required permission to the user by checking the box(The minimum access is to give overall read)

--> By default whatever we create users for jenkins will get stored in jenkins own user database.

--> This is suitable for smaller set up where you have no existing user database elsewhere.

--> The other option is LDAP(Light weight Directory Access Protocol)

## Authorization strategies

--> By default we will be seeing project-based matrix authorization strategy with this we can manage the authorization based on the options available under strategy.

EX: Credentials,Agents,job,run,view etc...

## Matrix Authorization strategy

## Use cases 

--> Matrix Authorization allows configuring the lowest level permissions,such as starting new builds,configuring items or deleting them individually.

## Jenkins Projects (Project/job)

--> It is a combination of one or more tasks.

1. Freestyle Project - A simple Jenkins job for automating tasks like builds or scripts.

2. Pipeline - A job that defines CI/CD workflows using a Jenkinsfile.

3. Multi-configuration project - A job running on multiple configurations with separate results.

4. Maven-Project - A Jenkins project for building Java applications using Maven.

5. Folder: A way to organize Jenkins jobs into a hierarchical structure.

6. Multi-Branch Pipeline: A pipeline that creates jobs for each branch in a repository.

7. Organization Folder: A folder that auto-discovers repositories and creates pipelines for each.


## RBAC(Role based access control)

 --> This is one of the way where we can secure the jenkins.

## How to create the Job/Project

--> In Jenkins GUI you will see the Plus symbol new item & click on that New item enter an item name/ Job name then select an item type once selectedany of the item click on ok button which will be highlighted.

--> The job Configuration is consists of( where we can give information/description about the project)

## Source code 

--> Source code management where will be passing URL'S of the repositories.

## Build Triggers

--> Build Triggers(In what way we wanted to trigger/build that job),build environment,build steps(where we can add tasks), post build actions.

## How to get Freestyle basic job

--> click on New item enter the job name select item type & click on Ok then once you configure.

--> Go to the build steps configuration of job click on add build step drop down button select execute windows batch command & select that just type dir & click save then click on build now & check for console output.

## BlueOcean

--> Blueocean rethinks the jenkins user experience designed from the ground up for jenkins pipeline & compatible with Freestyle jobs.

## What if jenkins user forgot the password

--> As a jenkins administrator there is a provision to reset the user credentials.

Manage jenkins --> security --> users

Go for the user which need to be reset & click on security.Once you click on security there you see the password & click on save.

--> Administrator if you change the password again you need to inform to the users saying please follow below steps to change the password.

--> Once logged in to the jenkins GUI click on username.Click on security there you can change the password & click on save.

--> In Jenkins slaves,agents,nodes these three terminologies are same.

## Jenkins Folder

--> In Windows OS we can see all the jenkins information & configuration details 

    c:\ProgramData\Jenkins\.jenkins\

--> Under .jenkins folder we can see users folder(where all the jenkins users data available)

## Workspace 

--> Where all the configured jobs information available.

## secrets

--> Where all the configured secrets are available.

## Plugins

--> All the plugins (which are installed manually & automatically) available.

## Nodes 

--> Where all the configured nodes are available.

## Logs 

--> We can see slaves(if configured) & tasks logs are available.

--> Apart from the above folders there is jenkins configurational file namely config.xml(If at all changing the config.xml) first take the backup of that or cop that file in someother folder.

--> we can also see the jenkins logs in jenkins GUI.

path: Managejenkins --> status information and then system log then all jenkins logs once click on that you will see all the details of logs.

--> We can see the jenkins version bottom right corner in Jenkins(GUI).

Path: Managejenkins --> status information then about jenkins.

--> Crontab.guru(https://crontab.guru/)

--> There are ways to trigger the jenkins jobs.

## Triggers
 
--> Set up automated actions that start your build based on specific events like code changes/ scheduled times. 

1. Trigger Build Remotely(Ex: From scripts)

--> In order to use this trigger first we need to generate the authentication token of the job.

EX: Enable this option if you would like to trigger new builds by accessing a special predefined URL (Convenient for scripts).

--> you will need to provide an authorization token in the form of a string so that only those who know it would be able to remotely trigger this projects builds.

--> This is most useful when your jenkins instance grants read access to this job to anonymous users.

--> when that's not the case, jenkins will reject requests sent to the trigger URL even when the correct token is specified.

--> Use the following URL to trigger build Remotely

JENKINS_URL/job/ajafreestle/build?token=TOKEN_NAME or /buildwithparameters?token=TOKEN_NAME

2. Build after other projects are built(Upstream and downstream jobs)

--> Set up a trigger so that when some other projects finish building, a new build is scheduled for this project. This is convenient for running an extensive test after a build is complete, for example.

--> We need to pass the job name (which are configured already) under projects to watch tab four options are available.

    1. Trigger only if build is stable

    2. Trigger even if the build is unstable

    3. Trigger even if the build fails

    4. Always trigger, even if the build is aborted

3. Build periodically (In Schedule)

--> This field follows the system of cron(with more differences) specifically, each line consists of 5 fields separated by TAB or whitespace.

MINUTE HOUR DOM MONTH DOW 

    MINUTE - Minutes within the hour (0-59)

    HOUR - The hour of the day (0-23)

    DOM - The day of the month (1-31)

    MONTH - The Month (1-12)

    DOW - The day of the week (0-7)

--> where 0 & 7 are sunday.

--> To specify multiple values for one field, the following operators are available. In the order of Precedence.

--> For reference or practise go with the website crontab.guru

4. Github hook trigger for GIT SCM polling

--> when jenkins receive a github push hook, github plugins checks to see whether the hook came from a github repository which matches the git repository defined in SCM/Git section of this job.

--> This option is available only GITHUB plugin is installed.

5. Poll SCM

--> Configure jenkins to poll changes in SCM.

--> Apart from the above five trigger options we can also triggers job manually.

--> Job configuration of build periodically trigger & poll scm trigger

--> Create new item (jon/project) go for triggers tab checkbox build periodically or pollscm. Once clicked on checkbox scheduling comment box will be open up.

--> There we need to schedule as per requirement.

Ex: To schedule a job at every minute,every hour on saturday 8th Feb.

--> where 1st * means every minute.

--> where 2nd * means every hour

--> where 8th is the day of month

--> where 2 is the month

--> where 6th is the day of week which is saturady.

--> Then click on save & check for the jobs whether running as per the schedule or not.

## Build after other projects are built

--> Create more than one job (yes) then in triggers option select build after other projects are built once you checkbox that option need to pass projects to watch name then click on save & check

Ex: Job1,job2,Job3 

--> For job2 put the upstream project as job1.

--> For job3 put the upstream job as job2.

--> when we build the job1, once job1 completed automatically downstream projects has to be build.

--> For job2 you select the build after other build other project built the select sub option trigger even if the build fails then save.

--> For job1 if we do mistake wantedly & check for all the jobs.

## Pipeline Project

--> We are going for pipeline project inorder to secure the CICD pipeline code by storing in any of the repositories (github,bitbucket & gitlab)

--> Sample Helloworld pipeline script creation

--> Click on new item select pipeline & click on ok.

--> Go for pipeline in configuration where we can define or write the pipeline script. We can write the script in script tab or else we can take it from SCM.

--> In the script tab click on dropdown option to try sample pipeline

pipeline {
  agent any

  stages{
    stage('Helloworld'){
      steps {
        echo 'Helloworld'
      }
    }
  }
}

--> Then Click on save.

--> Make sure that stage view plugin should be installed so that we can see stages.

## Rebuild vs Replay

--> When we use rebuild we are not changing anything but where as replay gives us provision to change the code then & there.

--> Replay we can also use it as one of the troubleshooting Mechanism.

--> If we don't know how to write pipeline script code we can take the advantage of snippet generator in pipeline syntax option(pipeline syntax option will only visible when you create pipeline job or project).

--> This snippet Generator will help you to learn the pipeline script code which can be used to define various steps. Pick a step you are interested in from the list, configure it.

--> Click generate pipeline script, & you will see a pipeline script statement that would call the step with that confihuration you may copy & paste the whole statement in to your script, or pick up just the options you care about.

EX: To Print message in sample step of snippet generator we can search for the echo/print you can search for echo.

 --> There is a step echo:Print Message then what message we want to print we have to pass it in message block then click on generate pipeline script which will give us script to print message.

 --> By default pipeline execution will work on serially (one by one). If the previous stages passed then only it will go for next stage or further stages.

## How to create new project/item from existing jobs

--> Click on new item

--> give the job name & select the item, scrolldown to bottom there you can see copy from option.

--> In that copy from we need to pass the job name which we want to make use of existing job configuration.

EX: create a Job10(Take the reference of Job8 configuration)

## How to change the default port number of jenkins

--> Go to the path c:\ProgramFiles\Jenkins in that folder find the jenkins.xml file

--> search for "--httpPort = 8080" in jenkins.xml file where 8080 is the default port number in order to change this default port number we should replace 8080 by our own port number then save it.

--> once modified this jenkins.xml files restart the jenkins server.

Note: Before changing any changes of jenkins configuration/port number better take backup of original file for safer side.

## What if jenkins administrator forgot the password

--> Go to the jenkins homedirectory c drive c:\ProgramData\Jenkins\.jenkins

--> In that path open config.xml file search for <useSecurity>true</useSecurity>

--> Replace True with False <useSecurity>false</useSecurity> then save it access the jenkins url in browser where you will not see any login details/user details in jenkins GUI & go for the manage jenkins 

--> First will go to security then under security Realm(where we change config.xml from true to false it will be none).

--> First here we need to change security realm from none to 'Jenkins own user database'

--> Next go for Authorization(where we change config.xml file from true to false authorization will change to Anyone can do anything)

--> Here we need to change from anyone can do anything to either Matrix based/project based strategy.

--> Once after changing the strategy under that uncheck the anonymous & click on Add user button & add the admin user & give the roll as administrator then save it.

--> We need to go for manage jenkins users go for the admin user change the password then save it. Now restart the jenkins server.

Note: Better take backup of config.xml

--> Once restarted check with admin user whether admin user has all the privileges or not then go back to config.xml file & modify use security tag from false totrue then restart the jenkins server.

## Using Jenkins environment variables

--> Jenkins pipeline exposes environment variable via the global variable env, which is available form anywhere within a jenkins file

https://www.jenkins.io/doc/book/pipeline/jenkinsfile/#using-environment-variables

--> Below are the some environment variables

1. Build_ID 

  --> The current BUILD ID, identical to BUILD_NUMBER for builds created.

  --> likewise we have BUILD_NUMBER,BUILD_TAG,BUILD_URL,JENKINS_URL,JOB_NAME,NODE_NAME then WORKSPACE

  --> For example user jenkins file(declarative pipeline) in that URL you will see basic example code copy that code create new item in jenkins for pipeline job.

  --> Replace the script with copied code & save it & build it.

  --> Expected output should be Running 1 on http://localhost:8080/

## How to parameterized the jenkins job

## Parameters

--> Parameters/variables allow you to prompt from one or more inputs that will be passed in to  a build.

--> Create New job in general configuration of that job you can see the option this project is parameterized need to checkbox that & there will use option add pareameter dropdown click on that you will see various parameters those are 

1. Boolean Parameter

2. Choice Parameter

3. Credentials Parameter

4. File Parameter

5. Multiline string Parameter

6. Password Parameter

7. Run Parameter

8. String Parameter

--> For example click on choice parameter(Defines a simple string parameter, which can be selected from a list. You can use it during a build) give thw name as ENV & under choice you can give more than one environment name & under description a description that will be shown to user later & click on save.

--> When you check the job to be trigger you will see build with parameter options.Click on that select the choices which we configured & go for the build button.

--> Another way of creating jenkins user

--> Manage jenkins then security checkbox the Allow users.

## Tools Configuration in Jenkins

--> If at all we wanted to configure tools like apache maven,docker e.t.c..

--> we need to go to the manage jenkins then system configuration then tools (configure tools,their locations and automtatic installers)

Ex: To configure apache maven specific version(3.6.0)

--> To configure apache maven in tools tab we should install plugin apache maven then onl we can able to see maven installations in tools.

--> Click on add maven then you can go for specific requirements.

--> To install automatically we should check the box install automatically option.

## How to trigger a job remotely

--> To configure this kind of requirement we can make use of trigger-trigger builds remotely using authentication token.

--> Create a freestyle job with name build remotely checkbox the trigger builds remotely option & configure an build step with authentication token(aja-123) save it & to check this job use the below URL.

Syntax remote URL: JENKINS_URL/job/buildremotely/build?token=TOKEN_NAME

--> Where JENKINS_URL is where jenkins is listening/accessible build remotely is job_name,TOKEN_NAME is authentication token which we configured.

    Ex: localhost:9999/job/buildremotely/build?token=aja-123

## Another way of triggering the job remotely

--> In Order to trigger job(EX:job2) we can go for the below command

    curl -u user<API_TOKEN> -X POST localhost:9999/job/job2/build

--> where -u is user(Tejaswini)(admin)

--> API_TOKEN which has to be generated with the user admin

--> POST is a method to call the URL'S.

# Linux

## What is Linux

--> Linux is an open source operating system modelled on Unix, & developed in c language.

--> Linux is more super fast compared to windows.

## Features of Linux

--> It is reliable as it runs smoothly & no need to reboot it repeatedly.

--> Huge base of developers that freely provides support.

--> Significantly reduces the monitory cost.

--> Linux is an open source

--> Licensing freedom to re-use & re-publish the code

--> Linux Can be customized if you want to change your system's look

--> New Enhancements happening & update come frequently

--> More secure than other operating systems.

## Where Linux is used

 * servers

 * super computers

 * Gaming & visual effect servers

 * Embedded systems

 * Android

 * NASA

## Components of Linux Operating system

## Init 