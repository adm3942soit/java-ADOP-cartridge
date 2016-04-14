     
"Java201-adop-cartridge"
========================


The DevOps Platform
===================
The DevOps Platform is a tools environment for continuously testing, 
releasing and maintaining applications. 
Reference code, delivery pipelines, automated testing and environments 
can be loaded in via the concept of Cartridges.

![home.png](https://raw.githubusercontent.com/accenture/adop-docker-compose/master/img/home.png)

[More details about DevOps](https://github.com/Accenture/adop-docker-compose)

**What is Cartridge?**
=======================

A Cartridge is a set of resources that are loaded for a particular project. 
They may contain anything from a simple reference implementation 
for a technology to a set of best practice examples for building, 
deploying, and managing a technology stack that can be used by a project.

This cartridge consists of list of repositories and jenkins jobs for work with them.

**Source code repositories**
============================

  Cartridge loads the source code repositories, which created in trening **"java201"**.
  This repositories added in file **repositories.txt**
  Each repository must be prepared for processing them in 
              **docker->DevOps->jenkins**

![docker_jenkins.png](https://github.com/adm3942soit/java-ADOP-cartridge/blob/master/docker_Jenkins.png?raw=true)
 
 
**Getting Started Instructions**
=================================
  1.Check please your gradle-project's file **"settings.gradle"** 
  in the root of your project with context:
  
                    rootProject.name='nameYourProject'
 
  2.Prepared permissions your project's gradle-files for linux-environment 
  of docker-machine:
                       
                       git ls-tree HEAD
                       git update-index --chmod=+x build.gradle
                       git update-index --chmod=+x gradlew
                       git commit -m "Changing file permissions"
  
  3.Add please your repository's url to file
                       
                       repositories.txt 
                       repositoriesGradle.txt
                       
                          
**Result building your project in Jenkins**
==========================================
  
![result_jenkins.png](https://github.com/adm3942soit/java-ADOP-cartridge/blob/master/result_jenkins.png) 
  
  
  **Successful building to you!**
  
  
  
  
  
  
  
  
  
  
  
      