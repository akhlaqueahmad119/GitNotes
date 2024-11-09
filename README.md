Git is a Software and Github is a online service.


<!-- About Git  -->

Let’s start with the basics. Git is a version control system that allows you to track changes to your files and collaborate with others. It is used to manage the history of your code and to merge changes from different branches.

<!-- Git and Github are different -->


Git is a version control system that is used to track changes to your files. It is a free and open-source software that is available for Windows, macOS, and Linux. Remember, GIT is a software and can be installed on your computer.

Github is a web-based hosting service for Git repositories. Github is an online platform that allows you to store and share your code with others. It is a popular platform for developers to collaborate on projects and to share code. It is not that Github is the only provider of Git repositories, but it is one of the most popular ones.


Before Git became mainstream, version control systems were used by developers to manage their code. They were called SCCS (Source Code Control System). SCCS was a proprietary software that was used to manage the history of code. It was expensive and not very user-friendly. Git was created to replace SCCS and to make version control more accessible and user-friendly. Some commong version control systems are Subversion (SVN), CVS, and Perforce.

<!-- Check your git version -->
git --version


<!-- Repository means folder -->
git status

<!-- Your config settings -->
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"

<!-- Now you can check your config settings: -->
git config --list

<!-- Creating a repository -->
git status
git init


<!-- WRITE -> ADD -> COMMIT -->


<!-- Commit -->
git commit -m "commit message"
git status


<!-- Logs -->
git log
git log --oneline 


<!-- change default code editor -->
git config --global core.editor "code --wait"


<!-- Creating a new branch -->
git branch
git branch bug-fix
git switch bug-fix
git log
git switch master
git switch -c dark-mode
git checkout orange-mode

Some points to note:

git branch - This command lists all the branches in the current repository.
git branch bug-fix - This command creates a new branch called bug-fix.
git switch bug-fix - This command switches to the bug-fix branch.
git log - This command shows the commit history for the current branch.
git switch master - This command switches to the master branch.
git switch -c dark-mode - This command creates a new branch called dark-mode. the -c flag is used to create a new branch.
git checkout orange-mode - This command switches to the orange-mode branch.


<!-- Note -->
Commit before switching to a branch
Go to .git folder and checkout to the HEAD file


<!-- Merging branches -->
git checkout main
git merge bug-fix


git checkout main - This command switches to the main branch.
git merge bug-fix - This command merges the bug-fix branch into the main branch.



<!-- Rename a branch -->
git branch -m <old-branch-name> <new-branch-name>


<!-- Delete a branch -->
git branch -d <branch-name>

<!-- Checkout a branch -->
git checkout <branch-name>

<!-- List all branches -->
git branch

<!-- Git Stash -->
git stash


<!-- Naming the stash -->
git stash save "work in progress on X feature"

<!-- View the stash list -->
git stash list

<!-- Apply the stash -->
git stash apply

<!-- Apply the specific stash -->
git stash apply stash@{0}


<!-- Applying and dropping the stash -->
git stash pop

<!-- Drop the stash -->
git stash drop


<!-- Applying stash to a specific branch -->
git stash apply stash@{0} <branch-name>

<!-- Clearing the stash -->
git stash clear
