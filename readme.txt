Hello Git and GitHub
The following notes are from: “Basic Git Workflow” Lesson

git init
initializes a local repository (makes a folder a git folder)

git status
checks the status of the folder
what has or has not been modified since the last commit

git add filename or git add .
adds files to the staging area (filename) or adds all files in repository (.)

git commit -m “info message here”
permanently stores changes in the staging area into the repository (local?)
checking status after commit should yield a “no new changes” type of message

git push -u origin master
pushes new versions/commits to the online repository on GitHub
“-u” option stands for “upstream”, establishes the link between local and remote repositories
only needed for the first push to the remote repository, used after “remote add” (below)

git push origin master
used to push successive commits/version to the remote repository
the local and remote repositories are connect, so “-u” options is not longer needed
can be used often and is the way files are back up to GitHub



Remote Repository Set Up & Checking Remote Connection

git remote add origin https://github.com/my-username/my-repository-name
specifies the GitHub online repository to be used with the local repository
used after first local commit

git remote -v
confirms remote has been added (fetch and push)
