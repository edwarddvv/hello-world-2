

**Show how to review repository commit history. (AC5.1)**

Use 

```git
git log 
```

to display the commit history for the current branch.

For a more concise version, use

```git
git log --oneline
```

And for a graphical display of the commit history, use

```git
git log --oneline --graph --decorate --all
```

**Describe why commit history matters (AC5.2)**

1. It shows the reasons for changes made (assuming descriptive commit messages)
2. It shows who made the changes
3. It shows when changes were made (so that if a bug is discovered, one can see how long it has been there)
4. If one wants to undo a change, one can find the point at which to revert the change

**Explain ways to undo changes. (AC5.3)**

If you have edited a file and you realise that you shouldn't have made those changes and you want to go back to the state of the file before you started then if your editor is still open, you could repeatedly press *undo*, but if you would have to press this too many times or you have already closed the editor, then run

```git
git checkout -- myfile.py
```
This will take *myfile.py* back to the version stored your local repository, so if you haven't commited, then all your changes will be undone.

If you made a mistake with a commit message, then you can change the message with

```git
git commit --amend -m 'Corrected message'
```

If you want to undo a commit, then you can use either *reset* or *revert*.  See below for the difference between these two commands.


**Describe the difference between reverting and resetting. (AC5.4)**

Revert sets the most recent version to be a previous version specified in the command. The version that was current is now the second last version.  Therefore, no change history is lost, but the changes that occurred after the point to which one reverts are ignored from this point forward.

Reset takes the local repository back to the specified point and dumps everything that is later.  Therefore, any changes that occurred after the point to which the respository is reset are lost.

