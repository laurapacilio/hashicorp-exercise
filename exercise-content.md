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
`git push` sends your local commits to the tracking branch in your remote repository.

Before you can push, you must update your local branch with the latest commits from the remote branch using either `git pull` or `git fetch` and then `git merge`. After you push, you may want to submit a pull request to merge your changes with the main development branch.
