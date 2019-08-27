# Introduction to git and the command line

This document contains some of the key information for how to use git in the command line. It has some of they key commands but by no means is extensive. A second document for the finer details with regards to bitbucket specific actions should be generated in a nearby file.

///-------BASIC COMMANDS-------///

$ git init      //initialise local git repository(generally hidden)

$ git add <file>    //add files to index

$ git status        //Check status of working tree

$ git commit        //commit changes to index/repository

// REMOTE REPOSITORYS
$ git push  //push to a remote repository

$ git pull  //Pull latest changes from remote reposity

$ git clone //Clone Repository into a new directory
 
 ////------INSTALLING GIT-------/////
$sudo apt-get install git

////-----EXAMPLE SYSTEM------////
 
 Create a new file in the desktop
 Git_Test in this case
 in the command line access the appropriate file, if unsure look at the terminal notes (yet to be made)
 --
 $cd        //highest level
 $cd Desktop
 $ ls       //Shows available file systems
 $cd Git_Test

 cmd line: ben@ben-XPS-13-9380:~/Desktop/Git_Test$

---- Create New files in this system -----

 $touch <filename>

 $touch app.js
 $touch index.html

 --- Open VSC----
 $ code

----Initialise the folder as a Git repository ----
$ git init
creates a (hidden) .git folder into the directory
(view options, show hidden files)


--Add name and email address to repository---
$ git config --global user.name 'Ben Molony'
$ git config --global user.email 'Ben_Molony@outlook.com'

--Add index html file to index repository
$ git add <filename>
--check its there
$ git status                //shows that index.html has changes to be commited
-- remove 
$ git rm --cached <filename>


------SPECIAL ADD------ 
$ git add *.<extension>   ///e.g. add*.html - adds all .html files to the internal repository
git add .  // adds everything

//////-------GIT COMMIT SECTION ----/////

$ git commit 
// takes to vim editor
i // insert mode

//Easier commit system
$ git commit -m 'Changed app.js'  //Comment to inc






