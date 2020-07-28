# Git Commands

## This repository contains frequently used commands for git

### **1. First time Git setup**

 File **GitInitialSetup.txt** contacts all the commands for initial configuration.

 Details steps are as below:

  Step 1: Login to your GitHub account in any browser

  Step 2: Jump to "Repositories" tab and click on "New" button

  Step 3: Create a repository with the specific name (without space) and select if you want to make it Public or Private

  Step 4: Once reposiroty is created, go to this newly repository and click on "Code" and copy the git URL

  Step 5: Now on your local machine, open a command prompt or terminal and navigate to the folder where you want to clone this newly created repository

  Step 6: Follow the below commands

   Clone the reposiroty with repository URL (This URL was copied in earlier step):
   * ```git clone https://github.com/<YourUser>/<YourRepositoryName>.git ```

   Navigate to the folder:
   * ``` cd <YourRepositoryName> ```
  
   Initial configuration
   * ```git config --global user.email "your_email@example.com" ```
   * ```git config --global user.name "myusername"  ```
   
   You are ready to make code changes
   * ```echo "123" > test.txt ```
   
   Check the status of your changes
   *  ```git status ```
   
   You would be able see the following output: <br/>
     ``` Untracked files: ```<br/>
     ```  (use "git add <file>..." to include in what will be committed) ```<br/>
     ```    test.txt ```<br/>
   
   
   Add your changes to git ("." indicates all files and foldes in current diectory should be added, if you want to add specific file then provide only that file name)
   * ```git add . ```
   
   Commit your changes with comments
   * ```git commit -m "initial commit" ```
   
   Push your changes to remote github repository
   * ```git push origin master ```
    
This complete your initial setup !!
