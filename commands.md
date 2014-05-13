
## First Steps
    git init
    git add .
    git commit -m "git commands - initial commit"

## Immer mal wieder zwischendurch

    git status
    (just to show the merge conflict:)
    added from person a
    added from person b


    git
## Github
- before second person clones, add them as "collaborator"

## History person A

    mkdir gitnotes
    cd gitnotes/
    subl commands.md
    ls
    git init
    ls -lart
    cd .git/
    ls
    ls refs/
    ls refs/heads/
    cd ..
    git status
    git add commands.md
    git status
    git commit -m "initial commit"
    git lg1
    ls .git/refs/heads/master
    less .git/refs/heads/master
    ls
    git status
    less .git/config
    git remote add origin git@github.com:htw-imi-info3/gitdemo_group2.git
    less .git/config
    git push
    git push origin master
    git status
    pwd
    git add .
    git commit -m "some more things"
    git status
    git lg1
    git push origin master
    git lg1
    git checkout -b feature1
    git lg1
    touch newfileinbranch.md
    subl newfileinbranch.md
    git status
    git add .
    git commit
    git lg1
    git checkout master
    ls
    touch createdinmaster.md
    git add .
    git commit -m "file added in master"
    git lg1
    git checkout feature1
    git rebase master
    git lg1
    git checkout -b newbranch
    touch newbranch.md
    git add .
    git comit -m "file in newbranch"
    git commit -m "file in newbranch"
    git status
    git push origin newbranch
    git checkout master
    subl .
    git add .a
    git add .
    git commit -m "line from person a"
    git push origin master


## History person B

    git clone git@github.com:htw-imi-info3/gitdemo_group2.git
    cd gitdemo_group2/
    git pull origin master
    git pull origin newbranch
    git branch
    git checkout newbranch
    git checkout master
    git pull origin master
    subl commands.md
    git add .
    git commit -m "line from person b"
    git status
    git lg1
    git push origin master
    git pull --rebase origin master
    git status
    subl commands.md
    git add commands.md
    git status
    git rebase --continue
    git status
