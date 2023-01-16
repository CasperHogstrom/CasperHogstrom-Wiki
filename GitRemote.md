# Working with git remotely

* ### Git clone
    Clones an existing repo into a new directory, good for testing without tampering with the "real" repo. ```git clone <URL>```

* ### Git pull
    Download content and updates your local repository to match the downloaded. Used when wanting the latest version from remote repo. ```git pull <branch name> <remote name>```

* ### Git push 
    Upload your local repository and commits to a remote one. Used to upload your work to a remote repo. ```git push <branch name> <remote name>```

* ### Git remote  
    Connects your local repo to a remote one. 
    Enables devs to work on the same repository by all having remote duplicates, needed for cooperative work on the same repo, in my experience so far. To add a connection to remote repo ```git remote add <branch> <URL>``` To check current remote connection ```git remote -v```

* ### Git merge
    Merge different branches, so called forked branches, into one. This is useful if work is done on different branches but then all work needs to be on the same branch. 
    
    To understand better ```git merge <branch name>```,  in this case develop so it will look like this, ```git merge develop```  Will result in the commit with the black dot. It creates a new commit along with the two commits that came before and a log message from the user describing the changes. Now the develop branch has merged into the main branch.

    ```mermaid
    gitGraph
        commit
        commit
        branch develop
        checkout develop
        commit
        commit
        checkout main
        merge develop
        commit
        commit
    ```