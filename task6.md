**Outline simple ways to stay in sync (pull regularly, check status, resolve conflicts, use branches, communicate changes). (AC6.1)**

Whether you are working with the main branch (just using the code) or a feature branch (changing the code), you should pull changes regularly.  With the main branch, you should be using the latest code because it will have bug fixes and you will be using the same code as everyone else.  With the feature branch, it is less work to merge your work in if you have been pulling changes from your colleagues.  You can use *git status* to see whether there are any changes that you've made that haven't been committed.  It is important to use descriptive commit messages so that other people know why you made the change and can decide when to merge it into their code.  

Sometimes when you pull the latest version of the branch that you are working on (with others), you find that a change has been made in a place that you have also modified.  This creates a conflict and you will have to compare the two changes to decide which one to retain (or possibly a combination of the two).


**Explain why staying in sync matters (avoids conflicts, prevents lost work, supports collaboration). (AC6.2)**

Pushing changes regularly has the following advantages:
1. If your hard disk breaks, you will lose less work because there will be a copy of the work of a remote server
2. Your collaborators are able to view your work and comment more often
3. The longer you wait to push a change, the more time there is for a colleague to make a change to that area of the file and cause a conflict

Pulling changes regularly means that it will be easier to combine your changes with the main code when the time comes to do so.
