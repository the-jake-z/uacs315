## Git Terminology
- **Clone**
	- Same as "Check out" in SVN, but it also creates a local repository for you computer.
- **Fetch**
	- Check if anything changed in the remote repository.
- **Stage (or Add)**
	- Approve changes that you want to commit.
- **Commit**
	- Commit the changes to the local repository.
- **Push**
	- Applies local commits to the remote repository.
- **Pull**
	- Gets the changes from the remote repository to the local repository.

## Workflow
1. "Clone"
2. Get changes from team members
	- Use "Fetch" to look at changes
	- Use "Pull" to apply changes to working directory.
3. Submit changes to remote repository
	4. _Stage_ to verify your changes
	5. _Commit_ to put it in your local repository.
	6. _Push_ to put it in the remote repository.

## Tools for CS 315

We're going to use the Git plugin that's built into Eclipse for our project. **All you have to do is install the lastest versions of Eclipse**.

## Setting up Git in Eclipse

For detailed instructions with screenshots, please view the lecture slides on [blackboard](https://ualearn.blackboard.com/bbcswebdav/pid-1844918-dt-content-rid-13806123_1/courses/45063.201540/1-Software%20Versioning.pdf).

## Conflicts
You will always end up with conflicts!

- If you don't work on the same file Git handles the conflicts for you while you **pull** the changes.
- If you work on the same file and both try to check in changes at the same time, there will be conflicts that will have to be reconciled manually.

#### Reconciling Manually

When you see conflicts, you will see them in the unstaged changes field in Eclipse.

To fix, right click the file in the unstaged commits changes and click the "Merge" option. This will open the conflicted file with differences highlighted in red.

Once you are done, you can stage the commit, and commit and push the same way that you check in files.

#### Strategies
- Try to avoid conflicts instead of merging them later because merging is tedious and error prone.
- Every now and then, before working on a project, do a "pull" first and keep synchronized with the remote repo.
- "push" frequently! 
- Conflict management is easier in text files, but binary files (images, videos, documents) are not possible to merge so you can either keep the remote copy or your copy.


