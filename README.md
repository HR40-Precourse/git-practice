# git-practice

This is a very simple tutorial that gives new Hack Reactor students who are unfamiliar with Git an opportunity to practice adding remote repos, pulling from remote repos, and resolving merge conflicts.

1. Fork this repo
2. Clone your fork of this repo (git clone <GITHUB_URL_OF_YOUR_FORK>)
3. Add this repo as an upstream remote (git remote add upstream https://github.com/HR40-Precourse/git-practice.git)
4. Add a remote to your pair's repo (git remote add <pairsName> https://github.com/<PAIRS_GITHUB_HANDLE>/git-practice.git)
  - you can always push work to your pair's repo with: git push <pairsName> master (or <branch name>)
5. Type git remote -v to see all the remote repos to which you have reference
6. Take a look at app.js
7. Let's imagine that your upstream remote has changed and you want to pull down the changes from it
  - Type 'git pull upstream changes' into the command line
  - (technically this pulls changes from a branch on the upstream remote called 'changes', most of the time you'd use git pull upstream master to pull from the master branch)
  - Notice how app.js has changed
8. Let's imagine that your pair leaves for a meeting and you want to continue working on the repo on your own, but don't want to overwrite anything. This is when you would cut your own branch (git checkout -b <branch name>)
9. In the new branch, change the name property to another name.
10. Now your pair is back so you'll want to checkout your local master again. Make another change to the name property of randomPerson that is different from the name you used in the other branch.
11. Commit and push your changes back to the origin master
12. Let's say you want to continue doing more work on your again, but you want the new changes that you made from the origin master that your pair and you were working on together. Check out your own branch (git checkout <branch name>) and then pull from the origin master (git pull origin master).
13. Your terminal should now be telling you that you have a merge conflict. Open app.js and delete the unneccessary lines to fix your conflicts. Then add and commit the changed file to continue the merge.
