# MergeRemotePractice
Q1- What does clone set the variable origin to represent?
it is cloning your remote repository. Origin represents your remote repostitory.

Q2- What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?
Origin is a variable that stores the remote repository URL and set upstream sets it. git push pushes your work to the remote repository and --set-upstream origin master sets where (what repository) you are pushing to. There are two separate branching structures (one local, one remote) Remote tracking lets you push and pull the correct things between these

Q3- Explain and illustrate what's happening in the commit tree when this command executes.
git pull origin master gets the commits from the remote master branch and then it merges origin/master into the branch you currently have checked out.

Q4- Are your commits overwritten by the remote master?
No because you merge master into your branch instead of merging your branch into master

Q5- Is this a merge or a rebase?
This is a merge because it doesn't override the project history

Q6- Person B: Checkout the local master branch- is it updated as well or still behind remote master?
It is still behind because when you pulled you pulled the remote master to the local branch not to the local master and thus the local master is still behind the remote master.  
