# Git and GitHub Cheat Sheet


## git config command
git config --global user.name "Your username"
git config --global user.email "Your email"

*Note: Using global ensures that every project on your computer will use those configurations

## Initializing a project

- Using the terminal, navigate to the location where you want to initialize the project.
- Run `git init`. You should receive a message similar to the following: "Initialized empty Git repository in `folder location`.
- Run `ls -la` command to display all the files created in the folder.

## Staging Files

- `git add FILENAME` - adds a specific filename
- `git add --all` - adds all of the files
- `git add -A` - is shorthand for adding all the files to staging
- `git add .` is even more shortand for adding all files to staging (only available on Linux)

Then commit what you have added to staging with the following:
- `git commit -m "My Commit"` - make your message a descriptor for what you are committing

Run `git log` to see a summary of what you've done.

## Git Environments

3 environments
- Working
- Staging
- Commit

File States
- Tracked
- Untracked - files that have not been added to the latest commit

Tracked files
- unmodified - unmodified since the last commit
- modified - files have been changed since the last commit
- staged

Discarding changes 
If you make changes to a file or files, use the restore command.

If you have made changes but not yet added to staging, then use one of the following:
- `git restore FILENAME` - restores a specific filename
- `git restore .` - restores all files
- `git checkout .` - an older version of the restore command

If you have made changes to a file and already added to staging, then use 
- `git resore --staged FILENAME` - use to move one file out of staging back into working
- `git retore --staged .` - moves all files out of staging and back into the working environment.

## Ignoring Files

Types of files you would want to ignore when committing:
- Files with sensitive information
- Files with personal notes
- Files with system files

Use .gitignore to specify the type of files you want to ignore.

Can also create a global ignore file that will work globally.

- `git config --global core.ecludesfile (file)`

### Clearing Cache

- `git rm - --cached .`


## Deleting and Renaming Files

Two ways to delete files managed by Git




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
