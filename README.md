


**Indepth-cli** is the client interface of an application whose goal is to fix defects in applications developed with the Java language (Indepth automates java code refactoring and remediation).

**Indepth-cli** analyzes your java source code on your workstation and automatically discovers bad development practices, defects or bugs (that are often referenced by Sonarqube). 
It also automatically applies patches in the source code.

**Indepth-cli** is very flexible. It allows you to determine the part of the project you want to analyze and fix it. 
The dry-run mode enables you to visualize the patches that Indepth would apply automatically.
You can also choose the issue you want to correct.

After the application of patches by Indepth, you should always test your app.

The **Indepth-cli** app is **free** to use on open source projects.

For more information please visit the website https://www.indepth.fr

### Why Indepth?

Software teams spend a significant amount of time trying to locate and fix bugs. 
Fixing a bug involves isolating the part of the code that causes unexpected behavior of the program and correcting the error. 
Bug fixing is a challenging task, and developers often spend more time fixing bugs and making the code more maintainable than developing new features.

**Indepth** was developed to face these challenges. Improve code quality quickly and carefully while letting developers develop value-added features.

The challenge is also economical. Indepth  can allow compagnies to reconcile the quality of the software assets with the needs of time to market.

### FEATURES

Java maven project remediation : issues are fixed automatically and systematically based on a specified rule.

Syntactic preservation : The original source code syntax is preserved.

Customization : You can choose the package you want to run a scan on or the rule to apply.

Security: You must register and log in to use Indepth and you can only see what you or what other people in your company have done.

Reporting: You can view the results of each execution at any time regardless of the execution mode (dry-run or not). You can view the changes in the form of diff.

To find out the details of the defects that Indepth fixes please visit the [project website](http://indepth.fr/documentation.html)


### INSTALLING & RUNNING

#### Installing

To install and run **Indepth-cli**, you need at least Java 8.

You need to download the latest version of the **Indepth-cli** application from https://github.com/javaperf-consulting/indepth/releases.

Copy the application to any directory.

Launch a console then move to the directory where **Indepth-cli** was copied.

Then launch **Indepth-cli** with the following command java -jar indepth-cli-&lt;version&gt;.jar

Watch the video 
https://www.indepth.fr/video/indepth_install_client_app.mp4

#### Create an account and setup a project

All you need to do when using Indepth for the first time is to register and create a project. A video is better than a long speech https://www.indepth.fr/video/indepth_setup_client_app.mp4

#### Running a code remediation

After the registration, you can signin (at the beginning of the session), then choose a rule to apply, run a remediation and show reports https://www.indepth.fr/video/indepth_running_example.mp4

### Indepth cli commands

```
Built-In Commands
       help: Display help about available commands
       stacktrace: Display the full stacktrace of the last error.
       clear: Clear the shell screen.
       quit, exit: Exit the shell.
       history: Display or save the history of previously run commands
       version: Show version info
       script: Read and execute commands from a file.

Project commandes
       license: Show license information
       signin: Signin
       unregister: Unregister user
       project: Create or update a project
       run: Run a remediation
       rules: Select a rule to apply
       exec: Displays information corresponding to the command [history|summary|details] respectively
        - The history of executions;
        - The summary of an execution;
        - The detail of an execution;
       register: Register new user
```

## Registration

You have to create an account before any use. 
Be careful because data will no longer be editable. 
They will be used to secure access to data resulting from code remediations.

## User profil

Overall there are 3 types of profile:

- during registration you are considered as a user wishing to test the application. 
You can use all features that do not require higher rights. 
But you will only be able to use Indepth in a demonstration mode which does not allow you to modify existing code. 
You will only be able to see what Indepth would have done if you had a commercial license. 
**For open source projects, code remediations are free of charge.**

- If your company has a commercial license, you will be able to modify to your code within the limits of the credits available on the company's license.
The features that you can use depend on your profile. 
If you are designated as a **solution administrator** you will have more possibilities than compagny users who are not an Indepth administrator. 
For example, as a **solution administrator** you can deregister users when they leave the company.
The designation of the administrator(s) is made when requesting your Indepth license.

## Project setup

The project must be developed in java. 
It has to be a Maven project. Gradle projects are not yet supported. 
Indepth can handle java versions from 8 to 18. 

You can also declare a git repository as source or a local directory on your workstation. 

If you are working on an Open source project, we invite you to set up the git repository otherwise your project will not be considered an Open source project and you will not be able to apply the modifications made by Indepth.

## Rules setup

Before launching a remediation you have to setup the rule to apply. 
You cannot currently specify multiple rules because we believe code remediation should be done very carefully.

## Start a code remediation

If you have a commercial license or if the project is open source, you can instruct Indepth not to apply code changes (dry run mode). 

In this case you will be able to observe the modifications that Indepth proposes. 

For commercial licenses (not open source projects) if you ask Indepth to apply changes in the code, credits will be consumed from the enterprise license. 
There will not be the possibility of canceling the consumption of credits.

You cannot currently launch multiple code remediations simultaneously in the same company.
This shouldn't be a problem because the runs only last few seconds or minutes.

## Reporting

You can analyze previous results at any time.
You can see the history of code remediation executions, or view a summary of an execution and even (in the form of a diff), the details of an execution (the code modifications made or suggested by Indepth).


## Start Indepth client application

Start Indepth simplest case

```
java -jar indepth-cli-<version>.jar
```

Start Indepth behind a proxy

```
java -Dhttp.proxyHost=<127.0.0.1> -Dhttp.proxyPort=<8888> -Dhttps.proxyHost=<127.0.0.1> -Dhttps.proxyPort=<8888> -jar indepth-cli-<version>.jar
```

### DOCUMENTATION

Read more at the [project website](http://indepth.fr/documentation.html), including more complete documentation.
