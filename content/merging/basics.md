Merging Basics
--------------

Once work on a branch is completed you can introduce those changes
into another branch through merging.

### Merging Branches ###

![](../../diagrams/branches/basic.tex)\
<!-- Placeholder -->

  * Work on the `feature` branch is complete

  * We would like commits `D` and `E` to move to the `master` branch

  * We will do this through merging

### Revisiting the Merge Base ###

![](../../diagrams/branches/basic.tex)\
<!-- Placeholder -->

  * The `feature` branch and `master` branch share a common ancestor

  * That ancestor is commit `B`

  * Git will perform a 3-way merge with `B`, `C`, and `E`

  * The result is a commit with two parents

### Merges Cause Multiple Parents ###

![](../../diagrams/merging/post.tex)\
<!-- Placeholder -->

  * A new commit is created: `F`

  * This is called a *merge commit* and has two parents

### Performing a Merge ###

  #. Switch to the destination branch:

        $ git checkout master

  #. Merge in the other branch:

        $ git merge feature

  #. Write a commit message in your text editor

### Exercise: Merging a Branch ###

  #. Change to the following directory:

        repos/basic

  #. Merge the `feature` branch into the `master` branch

(Hint: make sure you are on the `master` branch first.)