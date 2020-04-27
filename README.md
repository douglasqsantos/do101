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

## Initializing a Git Repository

## Objectives
After completing this section, you should be able to create a Git repository.

## Software Version Control
A Version Control System (VCS) enables you to efficiently manage and collaborate on code changes with others. Version control systems provide many benefits, including:

- The ability to review and restore old versions of files.
- The ability to compare two versions of the same file to identify changes.
- A record or log of who made changes at a particular time.
- Mechanisms for multiple users to collaboratively modify files, resolve conflicting changes, and merge the changes together.

There are several open source version control systems available including:
- CVS
- SVN
- Git
- Mercurial

## Introducing Git

Git is the most popularly used version control system. For this reason, you use Git as the version control system for all the exercises in this course.

Git can convert any local system folder into a Git repository. Although you have many of the benefits of version control, your Git repository only exists on your local system.

To share your repository with another collaborator, you must host the repository on a code repository platform.

There are many free code repository platforms, including:
- GitHub
- GitLab
- BitBucket
- SourceForge

In this course, you use GitHub to host and share your Git repositories.

### Git Workflow Overview

To retrieve the project files for an existing software project with Git, you clone the Git repository for the project.

When you clone a project, a complete copy of the original remote repository is created locally on your system. Your local copy of the repository contains the entire history of the project files, not just the latest version of project files. You can switch to different versions of the application, or compare two different versions of a file, without connecting to the remote repository. This allows you to continue implementing code changes when the remote repository is not available.

Git does not automatically synchronize local repository changes to the remote repository, nor does it automatically download new remote changes to your local copy of the repository. You control when Git downloads commits from the remote repository, and when local commits are uploaded to the remote repository. Git provides several mechanisms to safely synchronize your local repository with the remote project repository.

To track file changes in Git, you create a series of project snapshots as you make changes to your project. Each snapshot is called a commit. When you commit code changes to your repository, you create a new code snapshot in your Git repository.

Each commit contains metadata to help you find and load this snapshot at a later time:

- **commit message** - A high level summary of the file changes in the commit.
- **timestamp** - The date and time that the commit was created.
- **author** - A field that describes who created the commit.
- **commit hash** - A unique identifier for the commit. A commit hash consists of 40 hexadecimal numbers. If a Git command requires a commit hash to perform an operation, then you can abbreviate the commit to seven characters.

After you create commits in a local repository on your system, you must push your changes to the remote repository. When you push changes to a remote Git repository, you upload local commits to the remote repository. After a push, your commits are available for others to download.

When other contributors push commits to a remote repository, those commits are not present in your local repository. To download new commits from other contributors, you pull changes from the remote Git repository.

### Installing Git

Git is an open source version control system that is available for Linux, MacOS, and Windows systems. Before you can use Git, you must install it.

In a browser, navigate to https://git-scm.com/downloads and follow the directions for your operating system.

After installing Git on your system, you can use VS Code to manage your Git source code repositories.

To test your Git installation, open VS Code and access the integrated terminal (View → Terminal). At the terminal prompt, execute git --version. If Git is correctly installed, then a version number prints in the terminal:

### Configure the Source Control view in VS Code
Use the VS Code Command Palette (View → Command Palette...) and the Source Control view (View → SCM) to execute Git operations, such as cloning a repository or committing code changes.

By default, the VS Code Source Control view is different when you have one Git repository in your workspace, compared to when you have multiple Git repositories in your workspace.

When you have multiple Git repositories in your workspace, then the Source Control view displays a SOURCE CONTROL PROVIDERS list:

By default, when there is only a single Git repository in your workspace, then the Source Control view does not display the SOURCE CONTROL PROVIDERS list.

For a consistent user interface, independent of the number of Git repositories in your workspace, you must enable the Always Show Providers source control management option.

To enable this option, access the Command Palette (View → Command Palette...) and type settings. Select Preferences: Open Settings (UI) from the list of options. VS Code displays a settings window:

Click User, and then click Features → SCM. VS Code displays Source Control Management (SCM) options for VS Code. Select Always Show Providers

When you enable this option, then VS Code displays the SOURCE CONTROL PROVIDERS list in the Source Control view for any number of workspace Git repositories, including only one repository.

### Cloning a Git Repository

Use the VS Code Command Palette (View → Command Palette...) and the Source Control view (View → SCM) to execute Git operations, such as cloning a repository or committing code changes.

To clone a remote Git repository in VS Code, access the Command Palette (View → Command Palette...). Type clone at the prompt, and then select Git: Clone from the list of options.

VS Code prompts you for the URL of the remote repository, and then prompts for the desired location of the local repository on your file system.

After VS Code clones the repository, add the cloned repository folder to your VS Code workspace.

### Committing Code Changes

After adding a cloned repository to your VS Code workspace, you can edit project files like any other workspace files. As you edit project files, Git assigns a status to each file:

- **modified** - The file contains saved differences from the most recent version. Modified files are not automatically added or committed to your Git repository.
- **staged** - A staged file is a modified file that you flag to be included as part of your next code commit to the repository.

When you commit code to the repository, only those files with a staged status are included in the commit. If your project contains modified files that are not staged, then those files are not included in the commit. This feature enables you to control the file changes that are included in each commit.

In VS Code, the Source Control view (View → SCM) displays all modified and staged repository files. After you save edits to a file, the file name displays in the CHANGES list.

To add a modified file to your next code commit, click the modified file in the CHANGES list, from the Source Control view. VS Code displays a new tab to highlight the changes to the file:

If the file changes are accurate and complete, click Stage Changes to add the file changes to your next code commit.

After all of your desired file changes are staged, provide a commit message in the Source Control view. Then, select the check box to commit all of the staged file changes to your local repository.

### Using a Remote Repository

When you commit code changes, you only commit code to your local repository. No changes are made to the remote repository.

When you are ready to share your work, synchronize your local repository to the remote repository. To retrieve commits from the remote repository, Git performs a pull operation. To publish local commits to the remote repository, Git performs a push operation. VS Code handles the pull and push Git operations when you synchronize your local repository to the remote repository.

The Source Control view compares your local repository with the corresponding remote repository. If there are commits to download from the remote repository, then the number of commits displays with a download arrow icon. If there are local commits that you have not published to the remote repository, then the number of commits appears next to an upload arrow icon.

In the figure that follows, there

Click Syncrhonize Changes to publish your local code commits to the remote repository. Alternatively, you can click the same icon in the status bar to publish your code commits.

## Initializing a New Git Repository

If you have an existing software project that needs version control, then you can convert it to a Git repository.

To convert any file system folder into a Git repository, access the VS Code Command Palette (View → Command Palette...). Type intialize at the prompt, and then select Git: Initialize Repository from the list of options.

VS Code displays a list of project folders in the workspace.

After you select a project folder, Git initializes the folder as an empty Git repository. The Source Control view displays an entry for the new repository. Because the folder is initialized as an empty repository, every file in the project folder is marked as an untracked file.

For any project file that requires version control, click the plus icon to add the file to the local repository. Each added file displays in the STAGED CHANGES list in the Source Control view. After you stage all of the project files, provide a commit message, and then click the check mark icon to create the first commit in the repository.

When you create a new repository from a local file system folder, the new repository is not associated with a remote repository. If you need to share your repository:

- Create a new Git repository on a code hosting platform, such as GitHub.
- Associate your local repository to the new remote repository, and then synchronize changes.

Adding a Remote Repository to a Local Repository
After you create a new repository on a code hosting platform, the platform provides you with a HTTPS and SSH URL to access the repository. Use this URL to add this hosted repository as a remote repository for your local repository.

### NOTE
In this course, you only use HTTPS URLs to access remote code repositories. HTTPS access to a Git repository requires very little additional configuration, but does require that you provide credentials for the code hosting platform.

You can configure your Git installation to cache your credentials. This helps minimize re-entering credentials each time you connect to the remote repository.

SSH access to Git repository requires the configuration of your SSH keys with the code hosting platform.

SSH key configuration is beyond the scope of this course.

Access the VS Code Command Palette to add a remote repository to your local repository. Type add remote at the prompt, and then select Git: Add Remote from the list of options. If you are prompted to select a local repository, then make an appropriate selection.

At the prompt, enter origin for the remote name; origin is the conventional name given to the remote repository that is designated as the central code repository.

At the prompt, enter the HTTPS URL for your remote repository. If you have commits in your local repository, a Publish Changes icon displays in the SOURCE CONTROL PROVIDERS list.

Click the Publish Changes icon to push your local commits to the remote repository. If you are prompted, then provide the necessary remote repository credentials.

## For more information about installing Git, refer to the Git documentation at https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

[Git Basics](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository)

For more information about using Git and version control in VS Code, refer to the VS Code documentation at https://code.visualstudio.com/docs/editor/versioncontrol

## Guided Exercise: Initializing a Git Repository

In this exercise, you will use VS Code to push your project source code to a remote Git repository.

### Outcomes

You should be able to:
- Install Git.
- Initialize a local folder as a Git repository.
- Stage a file in a Git repository.
- Commit staged files to a local Git repository.
- Push commits in a local Git repository to a remote repository.
- You have access to a Linux (Debian or Fedora-based), macOS, or Windows system and the required permissions to install software on that system.
- Visual Studio Code (VS Code) is installed on your system.

### Procedure 1.2. Steps

- Download and install Git.
 - Linux Installation.
  - Open a new command line terminal.
  - To install Git on Ubuntu and Debian systems, use the following command:

## Git Branching

Basic Interaction
```bash
cd /path/to/project
git init
git add ./*
git commit -m "add code skeleton"
git add README.md
git commit -m "add draft README.md"
git add app.js
git commit -m "implement feature #1"
git add apps.js
git commit -m "fix feature #1 defect"
```

## Feature Branch

Basic Branch
```bash
git checkout -b feature2
git add
git commit -m "add feature #2"
git add
git commit -m "update dependencies"
```

# Git Merge

Merging
```bash
cd /path/to/project
git checkout -b feature2
git add
git commit -m "add feature #2"
git add
git commit -m "update dependencies"
git pull
git checkout master
git merge feature2
```

## NOTE

- Managing merge conflicts is beyond the scope of this course. For more information on merge conflicts, see Basic Merge Conflicts at https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
- Git tags are beyond the scope of this course. See Tagging in the Git documentation at https://git-scm.com/book/en/v2/Git-Basics-Tagging.

## NOTE
Often software projects adopt branch naming conventions or standards. Branch naming standards help you summarize the code changes contained in a branch.

The following are examples of branch name templates for a branch naming standard:

- feature/feature-id/description
- hotfix/issue-number/description
- release/release-string

A branch naming standard also defines the set of allowable characters. Branch names are often limited to alphanumeric characters and field seperators (such as /, _, or - characters).


## Login 

- https://mirror.openshift.com/pub/openshift-v4/clients/ocp/latest/

```bash
oc login https://api.cluster.domain.example.com:6443
```

```bash
oc new-project youruser-version
```

```bash
oc version
Client Version: 4.3.13
Kubernetes Version: v1.14.6+cd3a7d0
```

```bash
oc projects
You are not a member of any projects. You can request a project to be created with the 'new-project' command.
```

```bash
oc new-project dqs-version
Now using project "dqs-version" on server "https://api.ocp-la2.prod.nextcle.com:6443".

You can add applications to this project with the 'new-app' command. For example, try:

    oc new-app django-psql-example

to build a new example application in Python. Or use kubectl to deploy a simple Kubernetes application:

    kubectl create deployment hello-node --image=gcr.io/hello-minikube-zero-install/hello-node
```

The #update-app is the branch --context-dir is the folder inside the branch.

```bash
oc new-app --name version https://github.com/douglasqsantos/do101#update-app --context-dir version
--> Found image 0d01232 (7 months old) in image stream "openshift/nodejs" under tag "10" for "nodejs"

    Node.js 10.16.3
    ---------------
    Node.js 10.16.3 available as a container is a base platform for building and running various Node.js 10.16.3 applications and frameworks. Node.js is a platform built on Chrome's JavaScript runtime for easily building fast, scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.

    Tags: builder, nodejs, nodejs-10.16.3

    * The source repository appears to match: nodejs
    * A source build using source code from https://github.com/douglasqsantos/do101#update-app will be created
      * The resulting image will be pushed to image stream tag "version:latest"
      * Use 'oc start-build' to trigger a new build
    * This image will be deployed in deployment config "version"
    * Port 8080/tcp will be load balanced by service "version"
      * Other containers can access this service through the hostname "version"

--> Creating resources ...
    imagestream.image.openshift.io "version" created
    buildconfig.build.openshift.io "version" created
    deploymentconfig.apps.openshift.io "version" created
    service "version" created
--> Success
    Build scheduled, use 'oc logs -f bc/version' to track its progress.
    Application is not exposed. You can expose services to the outside world by executing one or more of the commands below:
     'oc expose svc/version'
    Run 'oc status' to view your app.
```

```bash
oc get pods
NAME               READY   STATUS      RESTARTS   AGE
version-1-2q9dc    1/1     Running     0          15m
version-1-build    0/1     Completed   0          18m
version-1-deploy   0/1     Completed   0          16m
```

```bash
oc logs -f pods/version-1-2q9dc                                                                                                    537ms  Mon Apr 27 14:11:14 2020
git version 1.8.3.1
Environment:
	DEV_MODE=false
	NODE_ENV=production
	DEBUG_PORT=5858
Running as user uid=1012300000(1012300000) gid=0(root) groups=0(root),1012300000
Launching via npm...
npm info it worked if it ends with ok
npm info using npm@6.9.0
npm info using node@v10.16.3
npm info lifecycle version@1.0.0~prestart: version@1.0.0
npm info lifecycle version@1.0.0~start: version@1.0.0

> version@1.0.0 start /opt/app-root/src
> node app.js

Server listening on port 8080...
```

```bash
oc get services
NAME      TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)    AGE
version   ClusterIP   172.30.91.85   <none>        8080/TCP   20m
```

```bash
oc get svc
NAME      TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)    AGE
version   ClusterIP   172.30.91.85   <none>        8080/TCP   20m
```

Exposing the service
```bash
oc expose service/version
route.route.openshift.io/version exposed
```

```bash
oc get routes
NAME      HOST/PORT                                           PATH   SERVICES   PORT       TERMINATION   WILDCARD
version   version-dqs-version.apps.ocp-la2.prod.nextcle.com          version    8080-tcp                 None
```

```bash
oc get all
NAME                   READY   STATUS      RESTARTS   AGE
pod/version-1-2q9dc    1/1     Running     0          19m
pod/version-1-build    0/1     Completed   0          22m
pod/version-1-deploy   0/1     Completed   0          19m

NAME                              DESIRED   CURRENT   READY   AGE
replicationcontroller/version-1   1         1         1       19m

NAME              TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)    AGE
service/version   ClusterIP   172.30.91.85   <none>        8080/TCP   22m

NAME                                         REVISION   DESIRED   CURRENT   TRIGGERED BY
deploymentconfig.apps.openshift.io/version   1          1         1         config,image(version:latest)

NAME                                     TYPE     FROM             LATEST
buildconfig.build.openshift.io/version   Source   Git@update-app   1

NAME                                 TYPE     FROM          STATUS     STARTED          DURATION
build.build.openshift.io/version-1   Source   Git@d41547f   Complete   22 minutes ago   2m39s

NAME                                     IMAGE REPOSITORY                                                                           TAGS     UPDATED
imagestream.image.openshift.io/version   default-route-openshift-image-registry.apps.ocp-la2.prod.nextcle.com/dqs-version/version   latest   19 minutes ago

NAME                               HOST/PORT                                           PATH   SERVICES   PORT       TERMINATION   WILDCARD
```

```bash
oc get routes
NAME      HOST/PORT                                           PATH   SERVICES   PORT       TERMINATION   WILDCARD
version   version-dqs-version.apps.ocp-la2.prod.nextcle.com          version    8080-tcp                 None
```

```bash
oc get pods
NAME               READY   STATUS      RESTARTS   AGE
version-1-2q9dc    1/1     Running     0          27m
version-1-build    0/1     Completed   0          30m
version-1-deploy   0/1     Completed   0          27m
version-2-build    1/1     Running     0          21s
```


```bash
oc logs -f version-2-build
Caching blobs under "/var/cache/blobs".
Getting image source signatures
Copying blob sha256:c48c210d99473f38a9f6e58c56cb5ec8674f3347c62917346a160e2bfbc43bde
Copying blob sha256:dfa32611d40bb3d014ffd60585c960f1c9b18070d438ad2886ac63f13ae80d19
Copying blob sha256:5af42566e7d1943de0196a7d22dc5abb18d916ae5cdb762dffd28d305a11ad41
Copying blob sha256:d49b8d97a29c461dfa980414df4295d43af55fc29fb51d63deba3df6198a8b91
Copying blob sha256:caa1771d2710f104d1441da00e8b236c3ba9cde637dc60c066bdb99ebe40412b
Copying config sha256:0d01232685c9e175e45b8a77bc9b96993b9f216b89a1d606aef66a766cf6ea0c
Writing manifest to image destination
Storing signatures
[...]

Pushing image image-registry.openshift-image-registry.svc:5000/dqs-version/version:latest ...
Getting image source signatures
Copying blob sha256:13c6191c4c2f516910badc505375a2769bae97e7409aceba76e53c830c84a166
Copying blob sha256:5af42566e7d1943de0196a7d22dc5abb18d916ae5cdb762dffd28d305a11ad41
Copying blob sha256:dfa32611d40bb3d014ffd60585c960f1c9b18070d438ad2886ac63f13ae80d19
Copying blob sha256:caa1771d2710f104d1441da00e8b236c3ba9cde637dc60c066bdb99ebe40412b
Copying blob sha256:d49b8d97a29c461dfa980414df4295d43af55fc29fb51d63deba3df6198a8b91
Copying blob sha256:c48c210d99473f38a9f6e58c56cb5ec8674f3347c62917346a160e2bfbc43bde
Copying config sha256:b6ad594b65673ac413b5cc7c2d9cfe53c914a0d71fb3be31dc72409cf7fe39f1
Writing manifest to image destination
Storing signatures
Successfully pushed image-registry.openshift-image-registry.svc:5000/dqs-version/version@sha256:7fcb415debd3197c5d3e65f51928fb50a8c5a0a5f2d7926db2baaacae2e2b946
Push successful
```

```bash
oc get pods
NAME               READY   STATUS      RESTARTS   AGE
version-1-build    0/1     Completed   0          33m
version-1-deploy   0/1     Completed   0          30m
version-2-7msbw    1/1     Running     0          24s
version-2-build    0/1     Completed   0          3m13s
version-2-deploy   0/1     Completed   0          35s
```

