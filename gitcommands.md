Git commands

Configure git at your local by 

-> git config --global user.email "<email>"
-> git config --global user.name  "<name>"

-> git init 

Go to github,create a repo,then copy the https link which ends
with ".git",after copying it do the following

-> git remote add origin <link you copied>

After that check whether the repo is remotely added or not by

-> git remote -v

Then add the files to staging by using the "git add ."

-> git add .

When you try to push your changes to the git,it will ask for 2 factor
authentication,so for that what we need to do is go to github.com/settings/generateaccesstoken
Select generate access token,get your access token and then do the following

##### remove the exisiting branch

-> git remove remove origin

##### add the new set as follows

-> git add remote origin https://<access_token>@github.com/<username>/<repo_name>

##### to check the status you can use the following command

-> git remote -v
