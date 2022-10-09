# Git versioning system

- **USE FOR EVERYTHING**

- keeps modifications made to your project over time - can go back to previous version if bug appears
- can use github as a backup/cloud for all your projects
- can share code easily with other researchers
- can contribute back to other open source projects
- can collaborate with other people easily
- simple set of commands can give you lots of power

## github

- service which allows users to upload their git repository
- public or private repositories
- share code with other users
- accept pull requests from other users
- share repository with other users

## terms

- clone
- init
- add
- commit
- pull
- status
- branch
- remote
- fetch
- stash

## creating a git repository

```bash
mkdir my_first_git_repo
cd my_first_git_repo
# create readme and python script
echo "# My First Git Repo" >> README.md
echo "print('Hello World')" >> hello.py
# initialise repository
git init
# add all files
git add .
# commit the staged changes
git commit -m ":tada: initial commit :tada:"
# add remote repo
git remote add origin main <URL>
# push commit to remote
git push origin
```

## cloning existing git repository

```bash
mkdir my_first_git_repo_clone
cd my_first_git_repo_clone
# clone repo to local machine
git clone <URL> .
```

## making changes to a git repository

```bash
cd my_first_git_repo_clone
# make a change to one copy of the git repo
echo "print('Hello again!')" >> hello.py
# add changed file
git add hello.py
# commit change
git commit -m "extra hello"
# push to remote repo
git push origin main
```

```bash
cd my_first_git_repo
# pull changes from remote to local
git pull origin
```

## other commands

```bash
git -h
```