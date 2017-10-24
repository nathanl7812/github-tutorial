# GitHub Tutorial

_by Nathan Lei_

---
## Git vs. GitHub
__Git__ - Git is used to keep track of changes done to your code.

__GitHub__ - With Git comes GitHub. GitHub is a website that does Git repository hosting. You can   put your changes that you have done using git and store them at Github.

*There is Git without GitHub, but there is no GitHub without git.*


---
## Initial Setup
1. First go onto *github.com* and create an account
2. Once you are logged on and on the main page press the little pixelated icon on the top right
3. Click __Settings__
4. Now click __SSH and GPG keys__
5. Then click the green box on the top right that says __New SSH key__
6. Open *c9.io* on another window and log in
7. On the top right there should be a little gear icon, click it
8. On the left there should be __SSH Keys Column__, click that
9. Now there should be 2 paragraphs of really long code, you want to copy the one on the bottom under __Connect to your private git repository__
10. Now go back to github and paste the code inside the __Key__ and type in a title for it such as "cloud 9"
11. After all that click __Add SSH Key__

### Your cloud 9 account is now linked to your github account.

---
## Repository Setup
* __Go into your terminal on Cloud 9__ (it should look like a box with code at the bottom of your c9 repo,
it should read **_(your_username):~/workspace $_**)
* __Create a new folder__ (type in **_mkdir file_name_**)
* __Go into the folder__(type in **_cd file_name_**)
* __Go to Github.com__
* __Click the + button on the top right, then new Repository__
* __Type in a name for the Repo then hit "Create Repository"__
* __Go under "…or push an existing repository from the command line"   
and copy the first line of code ONLY__(it should look like     
"git remote add origin git@github.com:username/filename.git")
* __Go back to Cloud 9__(type in "__git init__", then paste the code that you have previous copied)
* __Go to GitHub__(copy the line of code under the one you have previously copied)
* __Go back to Cloud 9__("paste the code")
#### Your repo on cloud 9 is now connected to your repo on github
---
## Workflow & Commands
```
pwd - Shows you where you are
ls - Lits everything in your folder
cd - Changes directory
mkdir - New folder
rmdir - Removes folder
touch - Creates file
rm - Removes file
rm -rf - Deletes everything inside a folder
mv (to rename) - Rename a file
mv (to move) - Move a file

git init - initializes git in our directory
rm -rf .git - To uninit git folder
git add file - Adds file to stage to be commited
git add . - Adds everything
git add --all - Adds everything including deleted files
git commit -m "message" - Take snapshots of files on stage. Quote is a message for your current commit which is present tense.
git add remote origin URL - Builds a bridge between c9.io and github
git push -u origin master - Pushes your commits to the github repository
git push - Sends commits up to your repo on git hub
git diff - See difference between your code now and previous code
git log - See past commits
q (while in git log) - quit
Git status - To see which files are stages to be commited
Git pull - Bring any changes from remote repo down to local
git checkout -- <file>... - to discard changes in working directory
git add <file>... - to update what will be committed
git reset HEAD <file>... - To unstage or undo the add
```
---
## Rolling Back Changes
#### If you already have a file inside your cloud 9 repo this is how you add, commit, and push to github 

1) Make sure your terminal says __username:~/workspace/foldername__
2) Type in __git add .__(When you have made a change)
3) Type in __git commit -m "a description of what you did in present tense"__   
(For example __git commit -m "edit"__)
4) Type in __git push__ (You can use this after everytime you commit or after a couple commits)