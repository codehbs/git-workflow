# Good Git Hygene
As a member of CODE, you'll likely do some of your work in teams -- and you know what that means: version control. For people who are new to working in git, we put together a sample workflow.

If you're not familiar with git, here's a good [overview on git on Quora](https://www.quora.com/What-is-git-and-why-should-I-use-it).

## Sample Workflow

- [ ] Name the branch after the feature you're creating:
`git checkout -b "your-initials/name-of-feature"` (you will need the quotes when you create a new branch name)

- [ ] Code your feature

- [ ] Check the status of your changes:
`git status`

- [ ] Add the feature updates:
`git add --patch`

- [ ] Then go back to the master branch:
`git checkout master`

- [ ] Pull down all changes from master:
` git pull origin master`. This is an important step! This makes sure you are handling all (if any) merge conflicts on your computer

- [ ] Merge the master branch with your feature branch:
` git checkout your-initials/name-of-feature` and then merge your branch: `git merge master your-initials/name-of-feature`. If you have conflicts, you will see an alert. Resolve the conflicts.

- [ ] Then push up your feature branch:
`git push origin your-initials/name-of-feature`. Note: never type `git push origin master`. [Don't be that person who pushes to master](https://8thlight.com/blog/sandro-padin/2015/06/08/help-i-just-force-pushed-to-master.html) :) 

- [ ] Create a pull request on GitHub. Ask a teammate to approve your request.
