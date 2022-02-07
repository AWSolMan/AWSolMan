# Appwrite Solution Manager Concept

## Prerequisites
* Appwrite creates an API for the Console Functions see [Feature Request](https://github.com/appwrite/appwrite/issues/382)


## Basic Idea
The basic idea of the AWSolMan is to manage Appwrite projects in a tree like way. So each buisness project consists of multiple appwrite projects which have certain restrictions and simulating different development progress of the buisness project.

The simple example here would be a three System/Project structure consisting of:
* Development
* Quality Ensurance
* Production

The way of usage in this case would be to do manual changes only to Development and move finished developments to the Quality Ensurance for testing purpose and after the test results are approved moving the hole new development to the Production system.


## Why is a third party software needed for this
At the moment Appwrite doesn't support any way of making a copy of a project. It doesn't even give you the possibility to make a backup only of the structure of a project without usage data. 

## Further Ideas
As the basic idea only includes a full project copy which is ok for a straight forward way but excludes more complex scenarios. There are some more sub features which are planned.

### Transport System
This feature brings the possibility to collect changes in transports which then can moved to other projects. This transports include objects the following objects are currently planned:
* Collections
* Functions
* Data (Documents, Files, Konfiguration)