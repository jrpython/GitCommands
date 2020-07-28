# Git Commands
This repository contains frequently used commands for git

1. First time setup for Git

 File GitInitialSetup.txt contacts all the commands for initial configuration.

 Details steps are as below:

  Step 1: Login to your GitHub account in any browser

  Step 2: Jump to "Repositories" tab and click on "New" button

  Step 3: Create a repository with the specific name (without space) and select if you want to make it Public or Private

  Step 4: Once reposiroty is created, go to this repository and click on "Code" and copy the git URL

  Step 5: Open a command prompt or terminal and navigate to the folder where you want to clone this newly created repository

  Step 6: Follow the below commands

   Clone the reposiroty:
    git clone https://github.com/<YourUser>/<YourRepositoryName>.git

   Navigate to the folder:
    cd <YourRepositoryName>
  
   Initial configuration
    git config --global user.email "your_email@example.com"
    git config --global user.name "myusrename"
   
   You are ready to make code changes
    echo "123" > test.txt
   
   Check the status of your changes
    git status

    Untracked files:
      (use "git add <file>..." to include in what will be committed)
        test.txt
   
   Add your changes to git (. indiactes all files and foldes in current diectory, if you want to upload specific file then add only that file name here)
    
    git add .
   
   Commit your changes
    git commit -m "initial commit"
   
   Push your changes to remote git repository
    git push origin master
    
This complete your initial setup !!
