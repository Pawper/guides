git --version				                     	Lists version of Git
git config --global user.name "(Name)"		Change username
git config --global user.email "(email)"	Change email
git config --list                         Lists config details
git config --global --list                Lists global config details
git config user.email	               			Lists config email
git help				                        	Git help menu
git help (command)	                 			Git help on a specific command
git init				                        	Initialize an empty git repo in current working directory
git branch                                Lists branches
git branch (branch name)                  Create branch - work on individual branch and test before merging to master
git branch --delete (branch name)         Delete branch
git add .			                        		Add all files/changes in working directory to stage
git add (filename)		                 		Add new or updated file in working to stage
git commit -m "(message)"		             	Commit stage to repo with message
git commit -am "(message)"			          Commits all working updates to repo (not renames/removals)
git log					                        	Lists commit history
git log --author="(user.name)"	       		Lists commit history of specific user
git status				                      	Lists branch, untracked (working; not in stage) and tracked (in stage) files
git diff				                        	Lists differences between working and repo
git diff --stage		                  		Lists differences between stage and repo
git rm (filename)		                   		Removes file from working, adds to stage to remove from repo (must commit)
git mv (filename/path) (filename/path)		Renames file, adds to stage to rename file in repo (must commit); also used for moving
git checkout (branch name)                Checks out branch to working (use to move between branches)
git checkout -- (filename)		          	Checks out file from repo to working (like reverting)
git checkout -b (branch name)             Creates a new branch and switches to it
git reset HEAD (filename)		             	Removes file from stage
git checkout (commit #)	-- (filename)	  	Checks out file from a specified commit from repo to working (must commit) (can just type first few digits of commit #)
git remote add (nickname) (url)		       	Adds a remote repo destination you can push to (e.g., a Github repo; must create it there first; github.com/name/repo)
git pull                                  Pulls from master
git push -u (nickname) (branch name)   		Pushes local repo to remote repo
git push --set-upstream origin (branch)   Sends pull request of branch to origin (github)
git merge (branch name)                   Merge current branch with specified branch
git stash                                 Save stage if you need to switch branches
git clone (remote name/url) (branch name)	Clone remote repo (branch optional) to local repo (login required)
git rebase                                ????
git show                                  ????

touch .gitignore                          Creates .gitignore file for git to ignore files (prefs, etc.). try gitignore.io
          .(directory)	                 	Ignores files in directory