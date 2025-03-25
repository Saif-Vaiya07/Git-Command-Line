# ~~Basic terminal command:-

#### Lists files and directories in the current directory  
```
ls 
```

####  Lists all files and directories, including hidden ones   
```
ls -a/dir -a
```

#### Changes the current directory  
```
cd <directory> 
```

#### Moves up one directory  
```
cd ..
```

#### Move to root  directory  
```
cd / →  
```

#### Prints the current working directory 
```
pwd →  
```

#### Creates a new directory  
```
mkdir <directory>
```

#### Creates a new file →  
```
touch <file>
```

#### Removes a file →  
``` 
rm <file>
```

#### Removes a directory and its contents →  
```
rm -r <directory>
```

#### Displays the contents of a file →  
```
cat <file>
```

#### Using to open a file in terminal →  
```
open (file name)
```

<br>

# ~~ SSH Key gentrator command:-

## ssh key - 
First, check if an .ssh directory exists in your local file system. If the directory exists, navigate to it. Otherwise, generate a new SSH key using the following command:

#### Generate new ssh key  →   
```
ssh-keygen -o -t rsa -C git-hub email
```

<br>  

# ~~Git configration command:-

#### For checking the current Git version →  
```
git --version  
```

#### Used when adding a command for all repositories →  
```
--global   
```

#### For checking Git configuration →  
```
git config   
```

#### gTo set up the configuration name →  
```
it config user.name "your_name"   
```

#### To set up the configuration email →  
```
git config user.email "your_email"   
```

#### For checking all configuration list items →  
```
git config --list   
```

#### For unset property →  
```
git config --global/--local unset (property)   
```

<br>

# ~~ Make working directory:- 

#### Creating/Initializes a new Git repository in the current directory → 
```
git init
```

#### Clones a remote repository to your local machine → 
```
git clone <repository_url> 
``` 


<br>

# ~~ Working directory to stagging are:-

#### Adds a file to the staging area →  
```

git add <file Name> 
```

#### Stage all changed file in directory and subdirectory →  
```
git add <file Name>
```

#### Adds all changes to the staging area →  
```
git add .
```

#### Directory wildcard →  
```
git add *.js
```

#### Directory & subdirectory wildcard →  
```
git add **/*.js
```

#### When a file in stagging state the we will check the diffrence → ` 
```
git add diff 
```

#### Checking the staging history →  
``` git status 
```

#### restore file / jump to previous poistion → ` 
```
git restore 
```

#### Unstage a file →  
```
git rm --cached <file Name>
``` 

<br>

# ~~ Stagging area to loacl repository:-

## - Commiting
#### For commiting →  
```
git commit -m "message"
``` 

#### Shows the commit history →  
```
git log
``` 

#### Shows the commit history in online → ` 
```
git log --oneline 
```   

#### At a time file will go in stagging area and then local repository →  
```
git add <File Name> && git commit -m "commit message"
``` 


## -Uncommiting
#### Uncommit a file / file will moved to staging area →  
```
git reset HEAD^
```

#### File will moved to Working directory →  
```
git reset --soft HEAD^
```

#### →  File will moved to outside of Working directory  →  
```
git reset --hard HEAD^ 
```


## - Commit Jumping
#### Display the recent (HEAD) commit details →  
```
git show  
```

#### Display the specific commit details based on commit id →  
```
git show <Commmit id 1st-7 character>
```

#### Display the specific commit detailsby order number →  
```
git show HEAD~2
```  

#### To jump a commit based on these commit id →  
```
git checkout <Commmit id>
```

#### To return recent commit →  
```
git checkout master
```

<br>

# ~~[.gitignore file]
#### Ignoring Specific Files: →  
```
secret-config.json
```

#### Ignoring by File Type: →  
```
*.log, *.tmp, *.json, *.css
```

#### Ignoring Directories: → 
```
node_modules/, dist/
```

#### Ignoring Files in Subdirectories:  →  
```
logs/*.log
```

#### Ignoring Everything Except One File: → 
```
dist/*, !dist/index.html
```

#### Comments: → 
```
# This is an comment
```

<br>

# ~~Alias
it means shortcurt of git code

git config --global alias.(keyword) "property" = 
```
git config --global alias.s "status"
```

### - for unset 
git config --global --unset alias.(keyword) =
``` 
git config --global --unset alias.s 
```

<br>

# ~~Check remote connection: git remote
#### shows the remote along with the url →  
```
git remote -v
```

#### Syntax →  
```
git remote add name ‹REMOTE_URL>
```

#### Example →  
```
git remote add origin https://github.com/anisul-lslam/life-story.git
```

####  Remove the Remote →  
```
git remote remove origin
```

<br>

# ~~Branch
#### Check the all git branches → 
```
git branch 
```

#### Create new branch →  
```
git branch name(feature1)
```

#### Switch to another branch → 
```
git checkout name(feature1)
```

#### Delete a branch (but at first we will need to switch another branch) →  
```
git branch -d feature1
```

#### Push code from feature1 →  
```
git push - u origin name(feature1)
```

#### At a time create a new branch & automatically switch to this branch →  
```
git checkout -b name(feature2)
``` 

#### feature2 will be merge with main branch →  
```
git merge name(feature2)
```
