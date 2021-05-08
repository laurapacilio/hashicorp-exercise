## What is the difference between fetch, pull, and push?
Git fetch, pull, and push are commands that help you understand and synchronize changes between a local and remote repository.

### Fetch

`git fetch` downloads all of the branches, tags, and changes from a remote repository into your local repository without changing your local files. This allows you to review changes before you add them into your work.

When you're ready, use `git merge` to integrate changes into your local working branch.

### Pull

`git pull` combines two actions into the same operation:
1. Download all of the branches, tags, and changes from a remote repository into your local repository. This is equivalent to performing a `git fetch`.

2. Integrate the changes from a remote tracking branch into your local tracking branch. This is equivalent to performing a `git merge`.


### Push
- `git push` - sent changes from a local branch to a remote repo

`git push` takes our current branch, and checks to see whether or not there is a tracking branch for a remote repository connected to it. If so, our changes are taken from our branch and pushed to the remote branch. This is how code is shared with a remote repository, you can think of it as "make the remote branch resemble my local branch". This will fail if the remote branch has diverged from your local branch: if not all the commits in the remote branch are in your local branch. When this happens, your local branch needs to be synchronized with the remote branch with git pull or git fetch and git merge.
