## Getting Started with GitHub
This document provides information on how to get started with GitHub, which is a provider of Internet hosting for software development and version control using Git. To leverage your experience and facilitate the management of assignments, we are using GitHub in combination with GitHub Classroom. 

GitHub Classroom tracks and manages assignments in your dashboard, grade work automatically and help students when they get stuck --all while using GitHub, the industry-standard tool developers use.

## Creating your GitHub Personal Account
You can create a personal account, which serves as your identity on GitHub.com, or an organization, which allows multiple personal accounts to collaborate across multiple projects.
For the purpose of working with the IBM Accelerate assignments, choose GitHub Free for personal accounts.


+ Go to: https://github.com/
    + If you want to create a new personal account, make sure you are currently signed out of GitHub.
+ Click on Sign up for GitHub.
+ Follow the prompts to create your personal account or organization.
   > Enter your email.
    Create a password.
    Enter a username.
    Click on Continue.
    Select your preference for product updates and announcements. For example: "n"
    Click on Continue.
+ Verify your account.
+ Click on Create account.
+ Check your email and enter the verification code. You can also click the link inside the verification email to start using GitHub.
+ You can start using GitHub. 

## Generating a New SSH Key and Adding it to the SSH-Agent
Follow the steps described [**here**](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) to avoid being prompted for a username and password (personal access token) when working with Git.

## Joining GitHub Classroom and Accepting your Assignment
+ Click the assignment link sent to you. 
+ If not already logged in to GitHub, log in to your personal GitHub account. 
+ You should see the below screen. Choose Skip to the next step. 
+ Choose to Accept this assignment. 
+ The repository for the assignment is now being configured. 
+ You should see the below screen after refreshing, and you can click on the light blue link to your new repository. 
+ You’re now ready to start the assignment. Read through the README for further instructions. 

## Clone and Import the Repository into the VS Code IDE
**Using the terminal:**
+ Download and install VS Code (if needed): https://code.visualstudio.com/download
+ Open a terminal on your computer.
+ Clone the repository: git clone https://github.com/2022-IBM-Accelerate-SW-Track/gh-classroom-test-<your-username>.git
+ Open your VS Code IDE.
+ Click on File > Open.
+ Search for the repository in your file system.
+ Click on Open.
+ The repository will open on your IDE.

**Using the GitHub Classroom VS Code extension:**
+ Go to the assignment repository.
+ Click on Open in Visual Studio Code. VS Code will be opened, and a prompt will appear on the screen.
+ Click on Install and Open.
+ Click on Open. You will receive a message saying, "The extension 'GitHub Classroom' wants to sign in using GitHub."
+ Click on Allow. Add your login information if prompted.
+ The repository will open on your IDE.

## Install and Run your Web Application
+ Open your VS Code IDE.
+ Click on Terminal > New terminal.
+ Select your repository.
+ Click on the Enter key.
+ A new terminal session will be started.
+ Go to your repository: cd gh-classroom-test-<your-username>.git
+ Run the following command: npm install
+ Run the following command: npm run dev

## Pushing your Code
In you VS Code IDE terminal
See status of your changed files 
`git status` 
**Add the files to be staged for commit**
`git add my_modified_file.js`
**Commit staged files**
`git commit -m "making my first commit"`
The git commit command create a new commit with all files that have been added. The -m "making my first commit" is the message alongside the commit used for future reference.
**Push your changes**
`git push -u origin <default branch>`
The -u flags sets the remote origin as the default. This lets you easily do a `git push` 
