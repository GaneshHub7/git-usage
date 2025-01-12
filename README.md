# wildlife-tracking-system

Create a github account with your personal gmail account

Create a repository for the project with proper naming convensions by github.
Ex : Wildlife-tracking-system

Local System setup :
    
    Create a specific folder to keep all your project dependencies.
        Ex : project tools kit
        
    Primary dependencies with no prior knowledge of which programing language will be used.
        Git
        TortoiseGIT
        BeyondCompare
        NotePad++
        
        Complete few tutorials under udemy on how to use above tools?
        
    Language used :
        Python
            Install python 3.11.<Stable.minorVersion>
            IDE : Install Pycharm Community version.
            
How to Clone the project from github to local system :
    - Generate ssh key
		ssh-keygen //cmd
    - Register ssh public key(ssh) to gitHub 
		C:\Users\Ganesh\.ssh>dir
		 Volume in drive C has no label.
		 Volume Serial Number is 6259-D09F

		 Directory of C:\Users\Ganesh\.ssh

		05-01-2025  20:27    <DIR>          .
		05-01-2025  20:27    <DIR>          ..
		05-01-2025  20:24               419 id_ed25519
		05-01-2025  20:24               104 id_ed25519.pub
		05-01-2025  20:27               828 known_hosts
		05-01-2025  20:27                92 known_hosts.old
					   4 File(s)          1,443 bytes
					   2 Dir(s)  186,919,116,800 bytes free

		C:\Users\Ganesh\.ssh>
    
- Download the project :
		Ganesh@DESKTOP-OR3P9LO MINGW64 /e/project
		$ git clone git@github.com:GaneshHub7/wildlife-tracking-system.git
		Cloning into 'wildlife-tracking-system'...
		The authenticity of host 'github.com (20.207.73.82)' can't be established.
		ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
		This key is not known by any other names.
		Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
		Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
		remote: Enumerating objects: 3, done.
		remote: Counting objects: 100% (3/3), done.
		remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
		Receiving objects: 100% (3/3), done.
		
- Create the Python Environment 
		To create a Python virtual environment with the name py_venv, you can follow these steps:

		Navigate to your project directory: First, make sure you're in the directory where you want to create your virtual 
                environment.

		cd /path/to/your/project
		Create the virtual environment: Use the following command to create the virtual environment with the desired name 
                py_venv:

		python -m venv py_venv
		This command will create a new directory called py_venv in your project directory.
		
		Activate the virtual environment: After creating the virtual environment, you'll need to activate it to start using it.

		On Windows:
		py_venv\Scripts\activate

		Deactivate the virtual environment: To deactivate the virtual environment, simply run:
		deactivate
		That's it! You now have a Python virtual environment named .wts_python_venv in your project directory.
		
- Create .gitignore to avoid pushing the py_venv to github.
- git basic commands
       1. Git Configuration:
          Before you start using Git, it’s a good idea to set up your configuration (name and email) so that your commits are attributed 
          to you.
           git config --global user.name "Your Name"
           git config --global user.email "youremail@example.com"
  
  2.Initializing a Git Repository
	git init

  3. Cloning a Repository
         git clone <repository-url>
  
      4. Checking Repository Status
          git status
        
       5. Adding Files
          You need to add files to the staging area before committing them:
            Add a specific file:
             git add <file-name>
           Add all changes (modified, deleted, and new files):
            git add .
  
     6. Committing Changes:
        git commit -m "message"

     7. Viewing Commit History:
           git log

     8. Pushing Changes to Remote Repository:
        git push origin <branch-name>
        git push origin main

    9.Pulling Latest Changes:
       Before you start working on your local repository, it’s a good idea to pull the latest changes from the remote repository to 
       avoid conflicts:
          git pull origin main

    10. Creating a Branch:
        git branch <branch-name>

    11.Switching Between Branches:
  	git checkout <branch-name>

    12.Merging Branches:
       If you have made changes in a different branch and want to bring them into your current branch, you need to merge them:
       Switch to the branch you want to merge changes into:
          git checkout main
       Merge the other branch into your current branch:
         git merge <branch-name>

   13.Deleting a Branch:
      git branch -d <branch-name>

   14.Moving files inside to folder:
      git mv [source] [dest]
