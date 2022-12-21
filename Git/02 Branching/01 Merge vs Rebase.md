# Merge vs Rebase

- Merge takes all the changes in one branch and merges them into another branch in one commit.
- Rebase says I want the point at which I branched to move to a new starting point

So when do you use either one?

## Merge
Let's say you have created a branch for the purpose of developing a single feature. When you want to bring those changes back to master, you probably want merge.

## Rebase
A second scenario would be if you started doing some development and then another developer made an unrelated change. You probably want to pull and then rebase to base your changes from the current version from the repository.
