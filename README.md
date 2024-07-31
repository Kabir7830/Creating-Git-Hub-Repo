# Creating-Git-Hub-Repo
This guide is for beginners who do not know how to initialize a Git repo and push it to GitHub

# 1.1 Installing Git

1) https://git-scm.com/downloads open the link and choose the platform that you have (windows, mac or linux)
   ![image](https://github.com/user-attachments/assets/4b5008ae-3ea2-4d57-80f7-dfcc4ff55519)
2) Download the installer or portable zip file according to your system config
   ![image](https://github.com/user-attachments/assets/4c789d4c-33b4-4585-b250-2db91415e750)
3) Run the installer and install the Git
   ![image](https://github.com/user-attachments/assets/78f8fb60-a4ad-4cd2-a8b5-ffdf60efa4ae)
4) To verify that the Git has successfully installed on your pc

   open PowerShell or Command Prompt and run the command given below
       git --version
   ![image](https://github.com/user-attachments/assets/b1f38b38-4702-4849-9ffd-e75d208b1b15)

   if you have any errors that means git is not properly installed on the PC. If you get the git version then congrats Git has been successfully installed.



# 1.2 Initializing a Git Repo

1) open the folder/directory where you want to initialize the Git repo

   For example we are going to initialize our git repo in a folder named "Test"

2) Open Powershell in your desired directory

    Shortcut to open powershell or cmd in your directory

   Hold shift and press right click anywhere in the folder/directory and click on "open powershell window here"
   ![image](https://github.com/user-attachments/assets/8fc0b92d-aa5e-4613-b36d-816a671089da)

   Now type the following command

         git init

   this will initialize a git repo in your directory (a .git folder will be created in the directory)

3) Now we need to need to Create a Git Repo on GitHub to save our upload/push the changes we will do for that
   Go to github.com and create your account
4) Now Create a new Repo on your GitHub Account
      ![image](https://github.com/user-attachments/assets/c742b66c-749b-42f9-8773-6ea5d0884eaa)

   click on New button

   Choose a name for your Repo
   
   Choose the Public or Private status

   Click on Create Repository button

   Copy the URL of the Your Git Repo you have just create

   You can find the link here

   ![image](https://github.com/user-attachments/assets/ae3b3462-3db3-4a25-947f-5a2c15c4b130)

   or

   ![image](https://github.com/user-attachments/assets/6f1c116b-3c19-466a-8b67-634fdab818ce)

   copy the HTTPS link

5) Now return to the powershell and connect the Git to the GitHub

   Set the username
         git config —global user.name "your-git-username"

   Set the Email
         git config —global user.email "email-address-registered-with-github"

7) Now lets connect the GitHub repo to our Local Git Repo

         git remote add origin <link-you-have-copied-in-step-4>

   You have connected the the repos

8) Now lets add the changes and commit them so that we can push them on GitHub

   Add the changed files (if you want to add all the changed files then use "." else type the name of particular file)

         git add .

   Commit the changes that you have made with a comment

         git commit -am "comment"

10) Now lets push the changes

         git push origin main


# 1.3 Cloning a Repo

For cloning a repo you must have Git installed on your system. (Refer 1.1 Installation Steps)

To clone a repo open a folder/directory where you want to clone the repository and open the terminal in that directory (powershell, cmd or other)

Copy the git repo link and type the following command
   
      git clone git-repo-link.git

Your repo has been cloned


# 1.4 Connecting the Existing Repo with other PC or folder

For connecting already existing repo to the other folder or PC follow the below given steps

1) Clone the repo (refer to 1.3 Cloning a Rep)
2) Now perform the step number 5 from 1.2 Initializing a Git Repo
3) Fetch the changes if any

     git fetch orign main

4) Now you can add and commit changes

Your repo is connected.

   







