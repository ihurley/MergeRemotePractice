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

Q7- Run git branch- did your local copy of your branch delete when Person A deleted the remote branch?
No it did not delete the local copy of the branch when the master was pulled down after the branch was deleted on gitHub

Q8- * commit 4ecf2c2cb5041f3b244151306b426ce6cb3ae46b (origin/Again)
| Author: Isabelle Hurley <ihurley19@ihurley19.local>
| Date:   Tue Sep 4 14:39:58 2018 -0600
| 
|     commiting changes to blank
| 
* commit 4293734132561da112f6620bae363e64c11a4fcd (origin/Feature2)
| Author: Isabelle Hurley <ihurley19@ihurley19.local>
| Date:   Tue Sep 4 14:27:38 2018 -0600
| 
|     commiting feature 2 changes
| 
* commit b9e00f3620431b5359c1119d2d8ab00957ccdf50 (HEAD -> master, origin/master, origin/HEAD)
| Author: ihurley <34346968+ihurley@users.noreply.github.com>
| Date:   Tue Sep 4 14:24:07 2018 -0600
| 
|     Update README.md
|   
*   commit 7d8e34cbedde655a215f97b524a6a60037289433
|\  Merge: be11141 2b59ce5
| | Author: ihurley <34346968+ihurley@users.noreply.github.com>
| | Date:   Tue Sep 4 14:21:40 2018 -0600
:
