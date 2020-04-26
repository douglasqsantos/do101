# Introduction to OpenShift Applications (DO101) introduces developers to Red Hat OpenShift Container Platform.

- https://rol.redhat.com/rol/app/courses/do101-4.2/pages/pr01

Red Hat OpenShift Container Platform is a containerized application platform that allows enterprises to accelerate and streamline application development, delivery, and deployment on-premise or in the cloud. As OpenShift and Kubernetes continue to be widely adopted by enterprises, developers are increasingly required to understand how to develop, build, and deploy applications with a containerized application platform. While some developers are interested in managing the underlying OpenShift infrastructure, most developers want to focus their time and energy on developing applications, and leveraging OpenShift for its simple building, deployment, and scaling capabilities.

Introduction to OpenShift Applications (DO101) introduces developers to Red Hat OpenShift Container Platform.

## Course Objectives
- Demonstrate the basic skills required to deploy, update, scale, and troubleshoot applications on OpenShift.
- Demonstrate a good understanding of the benefits of using OpenShift, and how to contribute to applications that are deployed on OpenShift.

## Audience
- Standard Developers
- Student Developers

Prerequisites
 - JB183 or equivalent programming experience.


## Orientation to the Classroom Environment

For this course, Red Hat Training has provisioned an account for you on a shared Red Hat OpenShift 4 cluster. When you provision your environment in the Red Hat Online Learning interface, the system provides the cluster information. The interface gives you the OpenShift web console URL, your user name, and your password.

DO101 is a Bring Your Own Device (BYOD) class, where you use your own internet-enabled system to access the shared OpenShift cluster. The following operating systems are supported:

 - Red Hat Enterprise Linux 8 or Fedora Workstation 30 or later
 - Ubuntu 18.04 LTS or later
 - Microsoft Windows 10
 - macOS 10.13 or later

You must have permissions to install additional software on your system. Some hands-on learning activities in DO101 provide instructions to install the following programs:
 - Visual Studio Code
 - Node.js
 - Git
 - The OpenShift CLI (oc)

Do not to install these tools prior to the day or this course if you do not already have them in order to ensure a consistent experience in the course.

Hands-on activities also require that you have a personal account on GitHub, a public, free internet service. One of the first hands-on activities instructs you to create this account if you do not already have one.

## Chapter 1. Configuring a Cloud Application Developer Environment

## Abstract

Goal
 - Configure a developer environment with a modern integrated developer environment and version control.
Objectives	
 - Edit application source code with Visual Studio Code (VS Code).
 - Create a Git repository.
 - Use version control to collaborate and manage application source code.
Sections
 - Developing Applications with Visual Studio Code (and Guided Exercise)
 - Initializing a Git Repository (and Guided Exercise)
 - Managing Application Source Code with Git (and Guided Exercise)
 - Developing Applications with Visual Studio Code

## Objectives
After completing this section, you should be able to edit application source code with Virtual Studio Code (VS Code).

## Integrated Development Environments
 - Software developers execute many different types of tasks during the software development life cycle of an application:
  - compile and build the source code
  - correct syntax errors
  - debug runtime errors
  - maintain version control changes to the source code
  - refactor source code
  - execute source code tests

In the past, developers used a collection of separate tools, such as editors, compilers, interpreters, and debuggers, to develop software applications. Inefficiencies arose from using separate tools, leading to the creation of Integrated Development Environments, or IDEs. IDEs improve developer productivity by integrating common software development tools into a single application. IDEs often integrate:
 - language-specific editors
 - code completion capabilities
 - syntax highlighting
 - programming language documentation
 - code debugging
 - source control management tools, such as Git, SVN, or Mercurial

Many modern IDEs support multiple programming languages. Using these IDEs, developers create applications in a variety of different languages, without needing to learn language-specific tooling, such as compilers and interpreters.

## Developing Software with VS Code

VS Code is a popular open source IDE that supports multiple languages, including JavaScript, Python, Go, C#, TypeScript, and more. It provides syntax highlighting, code completion, debugging, and code snippet capabilities, along with a plug-in framework that allows you to install additional functionality from a plug-in marketplace.

## In this course, you use VS Code to create, edit, and manage source code projects.

## Overview of the VS Code Interface

The VS Code interface contains five primary components:

## 