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

    Merging 


# Git Branching:
    - Main branch => master 
        - Main production branch
        - Anything in the master branch is always deployable!!

    - What happens when we create a new branch? 
        - Creates a snapshot of the current master branch
    - New branch => New feature/Contribution
        - An enviorment where we can try things out
        - Branch will not be mergered into master until it is reviewed (CODE REVIEWS)

# Git Pull Request and Merging:
    - Upon creation of a new branch
        - Initial commit: git push --set-upstream origin <demo-branch-name> (ADD A NEW BRANCH TO GIT REPO)
        - Follow git workflow above for alll other changes  