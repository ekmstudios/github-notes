# Git and GitHub Cheat Sheet

Using lab.github.com

github learning lab

GitHub Flow
Local Repository <-> GitHub
Pull project down to your local environment
Inside of our copy, everything is organized into branches
Each change lives on a branch
Master branch is a record of all the changes on the project, the Master branch is live on production

When making changes, we create a branch.
Once a branch is created and changes are made to that branch, you can commit those changes to the newly created branch.

After making all the changes we’ve made on our branch and we want to put on another branch, we do a pull request.

What a Pull Request Means
You want to show changes you’ve made and add them to the production branch on GitHub

Create a branch > Add Commits > Open a Pull Request > discuss and review commits > deploy from the branch > merge branch into master

Working Locally with the Command Line
Why the command line
- run all Git commands in their full functionality
- Knowing Git on the command line transfer over to other tools
- less likely to change

Preparing to use the command line
pwd - print working directory
cd - change directory
ls - list files in a directory
touch - create an empty file
mkdir - create an empty folder

Check if Git is installed
git - -version (don’t put a space between the dashes)

Setting up Git
Git Configuration Levels
- - system (system wide configurations that apply to all users on that computer)
- - global (configurations based at the user level)
- - local (configurations applied to a specific repository)

git config - - global user.name “Ekmstudios”
git config - - global user.email “errol@ekmstudios.com”

check settings
git config - - global user.name
git config - - global user.email

Use the up arrow key to get the last command


git init 
initializes empty Git repository

git status
check in on the status of your repo

git add index.html
add the file

git commit -m “Commit message”
make the commit you want

git log
gives you a history of commits

touch app.js
touch styles.css

touch creates these files

git checkout 

git branch <new branch name>
creates a new branch

git checkout newbranch
switches to the branch newbranch

git merge <name of branch>
to merge the changes into master


Create a new repository on the command line


Push an existing repository from the command line
git remote add origin https://github.com/ekmstudios/ReactSample.git
git push -u origin master
