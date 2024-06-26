

## Setup git account in cmd
```
    git config user.email @email.com

    git config user.name username

    git config user.password password
```
## To view global Git config
```
    git config --global --list / git config --list
```
## Change config globally user.name user.email
```java
// <!-- If you want to replace the wrong ones with the proper one: -->

    git config --global --replace-all user.name newUsername

// <!-- same applies for user mail: -->

    git config --global --replace-all user.mail newEmail.com

// <!-- Cloning a git repository -->

    git clone https://github.com/user/git-repo.git
```
## Branches
```java

                                        Create

// <!-- To list total branches -->
    
    git branch 
    
// <!-- To create a branch -->
    
    git checkout -b new-branch

// <!-- To push all your branches to the remote -->

    git push --all -u

// <!-- To push a new local branch to a remote Git repository -->

    git push -u origin new-branch



                                        Delete

// <!-- To delete a branch -->

    git branch -d branch-name

// <!-- To push a deleted branch in local to the remote -->

    git push origin --delete branch-name
    

                                Checkout, commit & push

// <!-- To checkout a branch -->

    git checkout branch_name

    git fetch

    git pull origin   

// <!-- To add & commit & push -->

    git add .
    git commit -m"commit message"
    git push / git push origin  //popup comes to signin in GitHub account using browser/token, choose browser

```


## To give a Tage
```java
// <!-- after commiting changes to local -->

    git tag -a v1.0 -m"latest verion"
    git push origin v1.0 / git push origin v1.0 develop
```

## To view difference between two commits

```
    git diff

    git diff --staged

    git diff 6878544 b6f5be5

    git diff develop main
```

# Undoing added changes (not committed)
```java
    git add .

    git stash
    
    git stash clear //Clears the stashed files
```

# Undoing last commit (that has not been pushed)

```java
    git add .

    git commit -m"commit message"

    git reset --soft HEAD~

    git reset --soft HEAD~3		//Reverts all three commits
```

# Undoing a Specific Commit (That Has Been Pushed)
```java
    git log --oneline

    git revert 1a8ae86 --no-edit

    git push

    git reset --soft HEAD~		//HEAD~ is the latest commit

    git push -f origin develop / git push -f origin branch

    git reset --soft HEAD~3		//Reverts all three commits

    git push -f origin develop / git push -f origin branch
```

# Reverting a merged commit which pushed to remote

```java
    git reset --merge a9fdeb5 / git reset --merge HEAD~1    //HEAD~ is the latest commit

    git push -f origin develop / git push -f origin branch
```