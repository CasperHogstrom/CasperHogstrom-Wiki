# 10 Most important Git Commands when workin locally
* Git init (Initialize new Git monitorer, always the first step.)

* Git status (Check status of current monitored repo.)

* Git commit (Saves staged changes, along with a short description to the local repository.)

* Git version (Checks your current version of git.)

* Git log/git log -follow[file] (List the version history for current branch or file)

* Git add (It stages a change to be included in your next commit)

* Git checkout/git checkout -b (Used to switch from one branch to another. Can also be used to create a new branch and switch to it.)

* Git branch/git branch [branch name]/git branch -d [branch name] (Used to list local branches in current repo. Can also be used to create and delete branches.)

* Git config (Set configuration values locally or globaly for repos.)

* Git diff/git diff -staged (See the file differences which are not yet staged. See the file differences between the files in the staging area and the latest version present.)

![](Flowchart.svg) 
graph TD
    A(Working Directory) -->|Git add| B(Staging Area)
    B -->|Git Commit| C(Local Repository)
    C -->|Git Push| E(Remote Repository)
    E -->|Git Pull| C