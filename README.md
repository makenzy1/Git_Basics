This is a repo to help understand basic git commands.

Starting a Git repository and committing changes involves the following steps:

   1. Initialize a Git repository in an existing directory:

     cd <directory>
     git init

Replace <directory> with the name of the directory that you want to turn into a Git repository.

  2. Stage and commit your changes:

     git add <file>
     git commit -m "Your commit message"

Replace <file> with the name of the file you want to stage and replace "Your commit message" with a meaningful message describing your changes.

  3. Push the changes to the remote repository using the git push command:

     git push origin <branch>

    Replace <branch> with the name of the branch you want to push the changes to. If you're pushing to the main branch, you can use main instead of <branch>.

**Here's a more detailed explanation:**

    Initializing a Git repository: Use the git init command in the terminal (or Git Bash on Windows) to turn an existing directory into a Git repository. 
    This will create a new .git subdirectory in the directory, which will store all the information about the repository, such as its commit history and configuration.

    Adding and committing changes: Use the git add command to stage changes in your files, and the git commit command to commit the changes to the repository's history. 
    The -m option allows you to specify a commit message that describes the changes.

    This will upload your changes to the remote repository, making them available for others to access. 
    Note that you may need to enter your username and password for the hosting service if you're pushing changes to a repository that you don't own.

Note that once you've committed changes to a Git repository, they are stored in the repository's history and can be retrieved at any time using the git log command. 
This makes it easy to revert to previous versions of the code if necessary.

**Common Git Commands:**
git init: This command is used to initialize a new Git repository. 
It creates a new directory called .git, which contains all the necessary files for keeping track of the codebase. This command is typically used when you are starting a new project and want to use Git to track the changes.

git clone: This command is used to create a copy of a remote repository on your local machine. 
It allows you to download a copy of a repository from a remote location and create a local copy of it. You can then make changes to the local copy and push them back to the remote repository.

git add: This command is used to stage changes for commit. It tells Git that you want to include certain files in the next commit. You can use this command to add individual files or a group of files.

git commit: This command is used to save changes to the repository. It creates a new "commit" that includes all the changes that have been staged with the git add command. 
Each commit includes a message that describes the changes that were made.

git status: This command is used to check the current status of the repository. It shows which files have been modified, which files have been staged for commit, and which branch you are currently on. 
This command is useful for getting a quick overview of the changes that have been made to the codebase.

git diff: This command is used to show the difference between the current version of a file and the last committed version. It shows the lines that have been added or removed. 
This command is useful for reviewing changes before committing them.

git log: This command is used to display the commit history of a repository. It shows a list of all the commits that have been made, along with the author, date, and commit message. 
This command is useful for reviewing the history of a repository and understanding how it has evolved over time.

git branch: This command is used to create, list, or delete branches in a repository. Branches allow multiple developers to work on the same repository simultaneously without interfering with each other. 
(The git branch -M main command renames the current branch to "main". The -M option stands for "move/rename" and is used to move or rename a branch in Git.)

git merge: This command is used to merge changes from one branch to another. It allows developers to combine the changes made in different branches and integrate them into the main branch.

git pull: This command is used to retrieve changes from a remote repository and merge them with the local copy. It fetches changes from the remote repository and then automatically merges them with the current branch.

git push: This command is used to upload changes to a remote repository. It sends changes made in the local repository to the remote repository, updating it with the new commits. 
(The git push -u origin main command pushes the "main" branch to the remote repository named "origin". The -u option sets the upstream branch for the current branch.)
