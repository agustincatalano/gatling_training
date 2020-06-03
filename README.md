# PERFORMANCE GATLING TRAINING
this is a training performance training project with Gatling and Scala

This performance project is implemented in Maven using Scala + Gatling on IntelliJ CE IDE 

# Installation 
* Clone the repo and run mvn clean package
* On IntelliJ we need to create the following Application runner:
  Main class: Engine
  JRE: 13 
  ![runner](https://user-images.githubusercontent.com/12161403/83635756-09c03600-a5a5-11ea-8076-390a4d664790.png)

 If the IDE generate the following error when run the test: 
 ```diff
 - Error: Could not find or load main class Engine
 - Caused by: java.lang.ClassNotFoundException: Engine
 ```
 The solution is: right click on Scala folder inside on the IDE --> Mark directory as --> Test Resources Root
 
 ```diff
 + right click on Scala folder inside on the IDE --> Mark directory as --> Test Resources Root
 + run mvn clean package
 ```
 # IMPORTANT
 INTELLIJ requires install as a external library scala sdk but version 2.13 is NOT supported ATM. Supported version is 2.12.6
