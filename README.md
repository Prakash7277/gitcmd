----------github----------

git config --global user.name "Your Name"
git config --global user.email "you@example.com"

PS E:\Angular\ecom> git init

PS E:\Angular\ecom> git remote add origin https://github.com/Prakash7277/ecom.git

PS E:\Angular\ecom> git status

PS E:\Angular\ecom> git add .

PS E:\Angular\ecom> git commit -m "first commit"

PS E:\Angular\ecom> git push -u origin main
		OR
PS E:\Angular\ecom> git push -u origin master

----------Upload Angular project on github (live)----------

PS E:\Angular\ecom> ng add angular-cli-ghpages

PS E:\Angular\ecom> git init

PS E:\Angular\ecom> git remote add origin https://github.com/Prakash7277/ecom.git

PS E:\Angular\ecom> git status

PS E:\Angular\ecom> git add .

PS E:\Angular\ecom> git commit -m "first commit"

PS E:\Angular\ecom> git push -u origin main
		OR
PS E:\Angular\ecom> git push -u origin master

PS E:\Angular\ecom> ng build --base-href "http://Prakash7277.github.io/ecom/"

PS E:\Angular\ecom> npx angular-cli-ghpages --dir=dist/ecom

-------------How do I pull my project from github?----------------

	git clone git@github.com:username/repo.git
 ------------How To find my github username-----------

	  git config --global user.name

------------How To find my github useremail-----------
 
	  git config --global user.email

------------Multiple GitHub accounts on the same computer?-------- 
step 1)  search on desktop 
     2)  credential manager
     3)  Windows Credentials
     4)  Generic Credentials
     5)  git:https://github.com
     6)  Remove

     8)  go to => Git Bash => opne
     9)  git config --global user.name Prakash7277
     10) git config --global user.email abc@gmail.com

 ---------------------------Branching----------------------
 
git branch			# List branches

git branch <branch_name>        # Create new branch

git checkout <branch_name>      # Switch to branch

git checkout -b <branch_name>   # Create & switch to new branch

git merge <branch_name>         # Merge a branch into current


------------------------------------------local all cmd-------------------------------------------------------------------------

pwd
# Print the current working directory

cd /D
# Change to D: drive (Windows)

mkdir GitDemo
# Create a new folder named GitDemo

cd GitDemo
# Enter the GitDemo folder

touch index.html
# Create an empty index.html file

ls -a
# List all files, including hidden ones like .git

git status
# Check git tracking status (shows untracked files or changes)

git init
# Initialize a new local Git repository in the folder

git add .
# Add all files to the staging area

git commit -m "first commit"
# Commit staged files with a message

git config --global user.name "Your Name"
# Set global Git username

git config --global user.email "you@example.com"
# Set global Git email

git remote add origin https://github.com/your-username/your-repo.git
# Link your local repo to GitHub

git push -u origin master
# Push to GitHub and set tracking for master (use `main` if your branch is `main`)

git config --global --unset user.name
# Remove the global username

git config --global --unset user.email
# Remove the global email

