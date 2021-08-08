# Git Commands

## This repository contains setup steps for git repository, how to connect to a repository from local and frequently used commands for git

### **1. First time Git setup**

 File **GitInitialSetup.txt** contacts all the commands for initial configuration.

 Details steps are as below:

  Step 1: Login to your GitHub account in any browser

  Step 2: Jump to "Repositories" tab and click on "New" button

  Step 3: Create a repository with the specific name (without spaces) and select if you want to make it Public or Private

  Step 4: Once reposiroty is created, go to this newly repository and click on "Code" and copy the git URL

  Step 5: On your local machine, open a command prompt or terminal and navigate to the folder where you want to clone this newly created repository

  Step 6: Now follow the below commands to connect to a repository from local

   Clone the reposiroty with URL (This URL was copied in earlier step):
   * ```git clone https://github.com/<YourUser>/<YourRepositoryName>.git ```

   Once above command is successfully completed, navigate to the folder:
   * ``` cd <YourRepositoryName> ```
  
   Initial configuration (One time setup)
   * ```git config --global user.email "your_email@example.com" ```
   * ```git config --global user.name "myusername"  ```

   You can veify your remote branch. This will show which branch is confugured for fetch and push:
   * ```git remote -v ```
   
   You are ready to make code changes, let us try to create a test file and try to check-in into the git repository:
   * ```echo "123" > test.txt ```
   
   Check the status of your changes
   *  ```git status ```
   ```
   Untracked files:
    (use "git add <file>..." to include in what will be committed)
      test.txt 
   ```
   
   Add your changes to git ("." indicates all files and foldes in current diectory will be added, if you want to add specific file then provide only that file name)
   * ```git add . ```
   
   Commit your to git changes with message ("initial commit" in below example)
   * ```git commit -m "initial commit" ```
   
   Push your changes to remote github repository
   * ```git push origin master ```
    
This completes your initial setup !!!

### **2. Setup .gitignore**

If you want to commit specific files and directories then you can ignore them when you make a commit.

For example log files, private keys or local cache files are required to be checked-in into git then you can incude those file extentions in the .gitignore file.

This file is at the root of the local repository.

```# ignore everything in the code/logs directory
code/logs/*

# except specfic directory      
!code/logs/python/

# ignore all *.class files
/code/java/*.class

# ignore .git and .ipynb_checkpoints folder
.git
.ipynb_checkpoints
```

### **3. Commit your changes to remote**

Once initial setup is completed,  you would like to commit new changes frequently. Below steps shows the process to commit and push your changes to remote git repository

1. Check the status of all the files which are changed on local
 * ``` git status ```
 ```
 Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
 ```
2. Add your changes to git
* ``` git add . ```

3. Commit your changes to git with comment
* ``` git commit -m "commiting .gitignore file" ```

4. Push your changes to remote github repository
* ``` git push origin master ```



### **4. Frequently used commands**

1. Get the latest changes from remote <br/>
 * ``` git pull origin master ```
