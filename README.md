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

---------------see the differences (changes)------------------
git diff
---------------To see hidden files including the .git folder:-------
ls -a
--------------shows the commit history of your Git repository----------------
git log
---------------------------docker---------------------------------------------
mkdir docker-webapp4
cd docker-webapp4
notepad index.html
notepad Dockerfile

FROM nginx
COPY index.html /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

docker build -t mywebapp4 
docker run -d -p 8080:80 mywebapp4
http://localhost:8080
