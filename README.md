Step 1: find a place you like for your directory for your project.

2: open git bash in the folder. This can be done by navigating to the folder, and 

right clicking on it then clicking "git bash here", I'm positive there is a command 

for navigation but this is simple for the time being

3: initialize git using command git init. This creates file inside your folder. 

Don't worry about what is inside.

4: configure git using commands: git config --global user.name 'Darren Kunz'
git config --global user.email 'dakunzman@gmail.com'
git add index.html

git status       this shows items in staging area. Since we added the index it will 

show up, but if you didn't add lets say app.js file it will show up aside from the 

staging area

git rm --cached index.html
git status will now show both untracked.
git add *.html will add any html files. git add * or . works for all files. 

5: commiting: git commit. hit i to insert any comments. esc to get out of comment 

mode. then ":wq" then enter to commit.

6: after commit any further changes must be re added to stage, and recommitted. A 

quick way to commit command is
git commit -m 'Your comment'

7: ignoring files. command is
touch .gitignore

open the file and type the name of the file you wish to ignore. To ignore a 

directory type /directoryname.

8: branching. 
git branch mybranch    will create a branch.
git checkout mybranch      will navigate to the branch.
you will still use git commit -m 'comment' when done.

9: merging branch to master:
git merge mybranch

10: add to github: go to github, log in, create a new repository. Follow steps on 

page, with specific attention to the command git remote add origin ...
now git remote command will show origin
now git push -u origin master   pushes to github



