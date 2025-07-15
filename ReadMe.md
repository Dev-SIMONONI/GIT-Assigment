#What is Version Control
Version control is a system that tracks and manages changes to code and Documents overtime, it allows team to contribute with each other, review pervious code and changes
one of the major use of version control is to track changes to files especially in soft ware development, allow teams to collaborate with each other effectively and manage different versions of code or project file the help for back-ups and recovery

#What is GIT & GITHUB
GIT: is a version control system for traacking changes in source code during software development.
GIT-HUB: is a web-based Git repositotry hosting service, whch offers all of the distrubuted revision control and source code mangements(SCM)functionality of Git as well as adding it owns functionality

#DIFFERENTS BTW GIT & GIT-HUB
GIT						GIT HUB
git is a software				Git-hub is a service
git is a command line tool 			Git-hub is a grahpical user interface
git is installed local on the PC		Git-hub is hosted on the web
git is maintanied by linux			Git-Hu is maintained by microsoft


#STEP BY STEP PROCEDURE ON HOW TO INSTALL AND CONFIGURATE THE GIT ON LINUX TERMINAL
step1-install git to the PC using the "sudo apt install git" use the git --version to check the version of git
step2-using the github account user name "git config --global user.name "username on git hub"
step3-Github account email address "git config --global user."emailgmail.com"
step4-enter "git config --list" to view user.name=username              user.email=useremail
step5-setup SSH for remote repositories using "ssh-keygen -t ed25519 -C "user@gmail.com"
step6-eval "$(ssh-agent -s)" using this it helps to keep track of users identity keys and their passphrases 
step7-ssh-add ~/.ssh/id_ed25519 here the user is allowed to use any number of server
step8-cat ~/.ssh/id_ed25519.pub the command will print out your SSH key on the terminal
#NOW USING GIT THE PC HAS BEEN CONNCETED TO THE GIT-HUB ACCOUNT REMOTELY


#NOW TO CREATE A DIRECTORY AND COMMIT IT TO A RESPORITATY IN THE GIT-HUB ACCOUNT
step1:mkdir directoryname in the terminal
step2:touch a file to the directory
step3-trying using the git status get "fatal: not a git repository (or any of the parent directories): .git"
git has not be commited using the "git log" command 
step4-using "git init" to create a respository of git in the directorty
step5-using "git status" now a no commits yet we appear on the terminal
step6:do "git add filename" to add the file name to the local directory 
step7: do "git commit -m "setup name user choice" the commit saves the file to the local resporitary and it get a serial number 
step8: go to thr git hub account create a repository name it whatever leave it as public and create
step9:copy the ssh key link of the resposrity 
step10:enter "git remote add origin git@github.com:user email" now the file has be remotely conncted to the github repository 

try to commit more changes
