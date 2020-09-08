# git_check

# How do you see the files changed within each commit using GitHub Desktop GUI?

You can trace changes to lines in a file and discover how parts of the file evolved over time.



With the blame view, you can view the line-by-line revision history for an entire file, 
or view the revision history of a single line within a file by clicking . 
Each time you click , you'll see the previous revision information for that line, 
including who committed the change and when.

# How do you see the contents of what changed within each file for a commit?

There are many occasions where you may need to get a list of files that have changed between 
commit X and commit Y.

This is surprisingly easy with Git and can be done with the SHA, tag or relative to HEAD.

Use the following command:

git diff --name-only <SHA, tag start> <SHA, tag end>
This will use the diff command but will only output the file names rather than the 
changes within each file.

# How do you revert (backout) a commit?

The easiest way to undo the last Git commit is to execute the “git reset” command with 
the “–soft” option that will preserve changes done to your files. You have to 
specify the commit to undo which is “HEAD~1” in this case. The last commit will 
be removed from your Git history.


# What does HEAD refer to in the context of git?

HEAD is a reference to the last commit in the currently check-out branch. 
You can think of the HEAD as the "current branch". 
When you switch branches with git checkout, the HEAD revision changes to 
point to the tip of the new branch.
