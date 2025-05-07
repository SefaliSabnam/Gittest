# GITTEST

This project demonstrates basic Linux operations, Git setup, branch management, SSH key handling, repository management, Maven project creation, and Java application development.

---

## Table of Contents

- [Project Structure](#project-structure)
- [Branches](#branches)
- [Files](#files)
- [Prerequisites](#prerequisites)
- [Basic Linux Commands](#basic-linux-commands)
- [Git Setup](#git-setup)
- [SSH Key Generation](#ssh-key-generation)
- [Repository Cloning and Branch Management](#repository-cloning-and-branch-management)
- [Maven Installation and Java Project Setup](#maven-installation-and-java-project-setup)
- [Running the Java Application](#running-the-java-application)
- [Pushing Changes to GitHub](#pushing-changes-to-github)
- [Command History](#command-history)

---

## Project Structure

GITTEST/
├── commands.txt
├── README.md
└── test.java

---


---

## Branches

This project includes the following Git branches:

| Branch Name | Purpose |
| :--- | :--- |
| `main` | Default branch for stable code. |
| `master` | Legacy branch, not actively used. |
| `feature1` | For development/testing of feature 1. |
| `feature2` | For development/testing of feature 2. |
| `feature3` | For development/testing of feature 3. |


---

## Files

- `commands.txt`:  
  A list of all Linux, Git, SSH, and Maven commands executed during the project setup.
  
- `README.md`:  
  Documentation for the project.

- `test.java`:  
  A basic Java test file.  
  This file likely contains simple Java code (e.g., a "Hello, World" program or basic logic) used for initial practice with Git and Maven.

---

## Prerequisites

- Linux server or local Linux environment
- Git installed
- Maven installed
- Java JDK installed

---

## Basic Linux Commands

```bash
su root
ls
cd GIT/
ls -la
hostname
w
pwd
ping google.com

## Git Setup

git -v
git status
git config --global --list
git config --global user.name "YottDhee"    #your git user name example- SefaliSabnam
git config --global user.email "jegadevan0079@gmail.com"   #your email id
git config --global --list

## SSH Key Generation

ssh-keygen -t rsa
cat /home/ec2-user/.ssh/id_rsa
cat /home/ec2-user/.ssh/id_rsa.pub

## Repository Cloning and Branch Management

# Clone Repository
git clone git@github.com:YottDhee/GIT.git #the repo name which you have created

# Create Directory
mkdir DevOps
cd DevOps/
git clone git@github.com:YottDhee/GIT.git  #the repo name which you have created

# Initialize Git
git init

# Create and Checkout Branch
git checkout -b REDMI-NOTE_13Pro+

# Add and Commit Changes
git add .
git status
git commit -m "REDMI-NOTE_13Pro+ first commit"
git push origin REDMI-NOTE_13Pro+

## Maven Installation and Java Project Setup

# Install Maven
yum list maven
sudo yum install maven
mvn -v

# Generate Maven Project
mvn archetype:generate -DgroupId=Demomvn -DartifactId=DemoMavenProject -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

# Navigate and Build Project
cd DemoMavenProject/
mvn clean install

##Running the Java Application

# Create a New Maven Project
mvn archetype:generate -DgroupId=com.yottdhee.app -DartifactId=my-java-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

# Build the Application
cd my-java-app/
mvn clean install

# Run the Application
cd target/
java -cp my-java-app-1.0-SNAPSHOT.jar com.yottdhee.app.App

## Pushing Changes to GitHub


git init
git branch
git branch -m development
git status
git add .
git commit -m "Redmi-1397 - Created a Maven Project"

# Connect to GitHub Remote

git remote add origin git@github.com:YottDhee/my-java-app.git
git remote -v

# Push to Remote
git push origin development

## History Commands

history
history | cut -c 8-


```
Note: Ensure your SSH keys are properly added to GitHub before attempting to push.