
<a href="https://www.indepth.fr"><img src="https://www.indepth.fr/img/logo-indepth-black-tr.png"></a>




**Indepth-cli** is the client interface of an application whose goal is to fix defects in applications developed with the Java language (Indepth automates java code refactoring and remediation).

**Indepth-cli** analyzes your java source code on your workstation and automatically discovers bad development practices or defects, bugs often referenced by the Sonarqube solution. 
It also automatically applies patches to the source code.

**Indepth-cli** is very flexible. It allows you to declare the part of the project on which you want to analyze and apply fixes. 
You can also run it in dry run mode and analyze the patches that would have been applied if you had asked them to be applied automatically.
You can also choose the issue you want to correct.


Be careful because although **Indepth-cli** is very carefully tested, the application can sometimes introduce bugs. 
It is therefore essential that you run your automatic or manual tests after modifying your application to verify that **Indepth-cli** has not introduced any bugs.


The **Indepth-cli** app is **free** to use for open source projects.

For more information please visit the website https://www.indepth.fr

### Why Indepth?

Software teams spend a significant amount of time trying to locate defects and fix bugs. 
Fixing a bug involves isolating the part of the code that causes unexpected behavior of the program and changing it to correct the error. 
Bug fixing is a challenging task, and developers often spend more time fixing bugs and making the code more maintainable than developing new features.

**Indepth** was developed to meet these challenges. Improve code quality quickly and thoroughly while letting developers develop value-added features.

For companies, the challenge is also on an economic level and makes it possible to reconcile the quality of the software assets with the requirement of time to market.

### FEATURES

Java maven project remediation : issues are corrected automatically and consistently.

Syntactic preservation : The original syntax of the source code is preserved.


### INSTALLING & RUNNING

To install and run **Indepth-cli**, you need at least Java 8.

You need to download the latest version of the **Indepth-cli** application from https://github.com/javaperf-consulting/indepth/releases.

Copy the application to any directory.

Launch a console then move to the directory where **Indepth-cli** was copied.

Then launch **Indepth-cli** with the following command java -jar indepth-cli-&lt;version&gt;.jar


Watch the video

https://www.indepth.fr/video/Install_indepth_client_app.mp4



	

### DOCUMENTATION

Read more at the [project website](http://indepth.fr/documentation.html), including more complete documentation.