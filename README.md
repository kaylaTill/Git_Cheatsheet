# Git-Hub Cheatsheet

# Github Workflow:
    Creating a new Repository: 
        - git init 
            - git add <reponame>
        - git clone vs git fork:
        - git fork/git clone:
    
    Commiting and Pushing changes:
        - stage changed with: git add
        - commit changes with: git commit
        - push changes with: git push 


    Pull Request:
        - Fork/Pull Model: provides a way to notify project maintainers about the changes you would like them to consider
        - Shared Repository Model: opens conversation/code reviews

    Deployment: 
        - Final Test: Test Deployment of feature before merging to master Branch



# Git Branching:
    Main branch => master 
        - Main production branch
        - Anything in the master branch is always deployable!!

    What happens when we create a new branch? 
        - Creates a snapshot of the current master branch
    New branch => New feature/Contribution
        - An enviorment where we can try things out
        - Branch will not be mergered into master until it is reviewed (CODE REVIEWS)

# Git Pull Request and Merging:
    Upon creation of a new branch
        - Initial commit: git push <--set-upstream OR -u> origin <demo-branch-name> (ADD A NEW BRANCH TO GIT REPO)
        - Follow git workflow above for alll other changes 

    Pull Request options:
        
    
# Editing Commit History:
    Git reset: 
        git reset HEAD ~<number of commits to undo>
        git reset: reset staging area to match most recent commit 
            + --soft 
                – The staged snapshot and working directory are not altered in any way.
            + --mixed 
                – The staged snapshot is updated to match the specified commit, but the working directory is not affected. This is the default option.
            + --hard 
                – The staged snapshot and the working directory are both updated to match the specified commit.

# Important Basic Git Commands:
    git pull origin master:  Bring all changes from the origin remote's master branch and merge them into the local checked-out branch
    git push: Push up all commits from local repo to remote repo
    git checkout HEAD~<num of prev commits>: checkout to the specified commit and view 
    git merge origin/master <branch>: merge multiple branches into local copy 

# Things to keep in mind:
    origin => refers to the repo
    origin master => refers to the main branch on origin
    origin/master => a remote branch ( A representation or a pointer to the remote branch -> "master" on the remote named "origin")


# Best Practices:
    Squash and Merge:  
        Goal: combine all commits into one commit and merge into the default branch. 
        Github Merge pull request with Squash and Merge option: Pull requests with squashed commits are merged using the fast-forward option (Squashes the pull request's commits into a single commit)
        Default Github Merge pull request: Under the hood with --no-ff option. 

    Multilined commit messages:
        Terminal code editor set to nano:
            ctrl + o => saves current changes
            ctrl + x => saves commit changes and props submission screen

    
