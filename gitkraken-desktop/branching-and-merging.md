---

title: Branching and Merging
description: Learn about branching and merging in GitKraken Desktop.
taxonomy:
    category: gitkraken-desktop

---

Learn how to branch and merge in GitKraken Desktop. 🌳 🔀

<div class='embed-container embed-container--16-9'>
    <iframe width='560' height='315' src='https://www.youtube.com/embed/8-qRKyy-v7I?rel=0&vq=hd1080' frameborder='0' allowfullscreen></iframe>
</div>


Looking for a sharable summary? Learn about [how GitKraken solves merge conflicts](https://www.gitkraken.com/developer-problems/merge-conflicts?product=gitkraken&source=help_center).   

***

## Branches
When starting work on a new feature or bug, <a href="https://gitkraken.com/learn/git/problems/create-git-branch?product=gitkraken&source=help_center" target="_blank">create a new branch</a>. Right-click on any existing commit to create a branch:

<img src="/wp-content/uploads/add-branch-2025.png" srcset="/wp-content/uploads/add-branch@2x.png 2x" class="help-center-img img-bordered">
A branch is a pointer to a specific commit in the repo.

Branches allow you to isolate new work from other areas of the repository, and interact with other collaborators. If you're looking for direction, consider implementing <a href="/git-workflows-and-extensions/git-flow">GitFlow</a> as a merging strategy.

### Checking out branches
Branch checkout updates files in the working directory to reflect the version defined by that branch.

New commits are added to the currently checked out branch. If you find yourself on the wrong branch, <a href="/gitkraken-desktop/stashing">stash</a> your changes, switch to the correct branch, and then *pop* the stash.

When you create a new branch, GitKraken Desktop will automatically checkout the branch for you:

<figure class='figure center'>
    <img src='/wp-content/uploads/add-branch-2025.gif' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Right click to create a new branch.</figcaption>
</figure>


To checkout a different branch, double-click on the branch label on the Left Panel or via the Commit Graph.  Checkout is also available by right-clicking a branch.

### Rename a branch

Rename a branch by right-clicking the branch tag in the Commit Graph (or right-click the branch in the branch list on the Left Panel) and selecting `Rename branch-name`.

<img src="/wp-content/uploads/rename-branch.png" srcset="/wp-content/uploads/rename-branch@2x.png 2x" class="help-center-img img-bordered">
For hardcore keyboard warriors, you can also rename a branch using the Command Palette (Cmd+P or Ctrl+P) and type `Rename Branch`.

<img src="/wp-content/uploads/rename-branch-command-palette.png" srcset="/wp-content/uploads/rename-branch-command-palette@2x.png 2x" class="help-center-img img-bordered">
Note: You can only rename the current branch you are on.
### Delete a branch

To <a href="https://gitkraken.com/learn/git/problems/delete-local-git-branch?product=gitkraken&source=help_center" target="_blank">delete a branch</a>, right-click the branch and select `Delete {branch-name}`. You cannot delete a branch that is checked out, so be sure to first checkout a different branch to then delete it. 

To delete multiple local branches in the Left Panel, hold <kbd>Shift</kbd> then click to select a range of branches or hold <kbd>&#8984; | Ctrl</kbd>  then click to select specific branches. Then right-click to access the delete option.

<img src="/wp-content/uploads/multi-delete-branches.gif" class="help-center-img img-bordered">
<div class='callout callout--warning'>
    <p><strong>Caution:</strong> Deleting a branch is a destructive action.</p>
</div>

***
## Merging

Merging takes the commits on two different branches and combines them.

With a merge, files are automatically merged unless there are two conflicting set of changes, i.e. commits on the different branches updating the same line in different ways.

Drag and drop one branch onto another to initiate a merge, or just right click the branch you would like to merge in and select merge from the menu.

<img src="/wp-content/uploads/merge-right.png" srcset="/wp-content/uploads/merge-right@2x.png" class="help-center-img img-bordered">
<div class='callout callout--warning'>
    <p>Note 📝 - The in-app merge conflict output editor is only available with a <a href="https://gitkraken.com/pricing?product=gitkraken&source=help_center" target=_blank>Paid</a> license. </p>
</div>


### Choose your own adventure
* I want to merge my own stuff in -- Continue onward!
* I want someone else to review and merge for me -- You want a <a href="/gitkraken-desktop/pull-requests">Pull Request</a>!


### Merge Conflict Editor

Merge conflicts may happen when team members make different changes to the same line of the same file, or when one team member edits a file and another deletes the same file. Oops!

When collaboration goes wrong, GitKraken Desktop Merge Conflict Editor is here to clear the murky waters.

If your merge attempt triggers a merge conflict, GitKraken Desktop display the conflicting files in the Commit Panel.

<img src="/wp-content/uploads/merge-conflict.png" srcset="/wp-content/uploads/merge-conflict@2x.png" class="help-center-img img-bordered">
Clicking a conflicted file opens the _Merge Tool_.

The current branch is on the left, and the target branch that you're merging into is shown on the right. The _Merge Tool_ output is at the bottom.

<img src="/wp-content/uploads/merge-tool2.png" srcset="/wp-content/uploads/merge-tool2@2x.png" class="help-center-img img-bordered">
Each conflict section has a checkbox. Checking a section adds it to the **Output** at the bottom so you can see the options in context to decide which makes the most sense to commit.

<img src="/wp-content/uploads/merge-tool-toggle.gif" class="help-center-img img-bordered">
You can also mouse over the line number and click <button class='button button--success button--ui button--nolink'>+</button> to select specific lines for the  Output, or edit the Output window directly.

Clicking the up and down arrows will move you to the next conflict.

<div class='callout callout--basic'>
    <p><strong>Tip</strong> - Use the keyboard shortcut <kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>F</kbd> to search any of the 3 diffs inside the merge tool. </p>
</div>

<div class='callout callout--warning'>
    <p>Note 📝 - The in-app merge conflict output editor is only available with a <a href="https://gitkraken.com/pricing?product=gitkraken&source=help_center" target=_blank>Paid</a> license. </p>
</div>

<figure class='figure center'>
    <img src='/wp-content/uploads/merge-tool-gif.gif'>
</figure>

After the conflict is resolved, save the output and commit the changes.

<div class='callout callout--basic'>
    <p>Watch our Learn Git Tutorial on <a href="https://www.gitkraken.com/learn/git/tutorials/how-to-resolve-merge-conflict-in-git?product=gitkraken&source=help_center" target="_blank">how to resolve merge conflicts in git</a>.</p>
</div>


### External merge tools
Configure GitKraken Desktop to launch your tool of choice by navigating to <em class='context-menu'>Preferences <i class='fa fa-caret-right'></i> General</em>:

<img src="/wp-content/uploads/configureExternalTool.png" srcset="/wp-content/uploads/configureExternalTool@2x.png" class="help-center-img img-bordered">
GitKraken Desktop currently supports the following merge tools:

* Beyond Compare
* FileMerge
* Kaleidoscope
* KDiff
* Araxis
* P4Merge

If your merge tool from the list above is installed and is not showing up in the dropdown, then look for an option to install command line tools.

<img src='/wp-content/uploads/beyond-compare.png' srcset='/wp-content/uploads/beyond-compare@2x.png 2x' class='img-bordered center' style="display: block; margin-left: auto; margin-right: auto;" />

GitKraken Desktop does _not support_ the following merge tools:

* Meld
* SemanticMerge
* TortoiseMerge
* WinMerge

While GitKraken Desktop allows Git Config Default merge tools, not all tools will be compatible. Find more information about configuring a <a href="https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration#_external_merge_tools">default merge tool in your Git Config</a>.

### Resolving a conflicted file using current or incoming

You may resolve a conflicted file by right-clicking the file in the commit panel and selecting the option `Take current (branch)` or `Take incoming (branch)`.

* `Take current (branch)` will apply the changes of the current branch.
* `Take incoming (branch)` will apply the changes of the incoming branch.

<img src='/wp-content/uploads/current-incoming.png' class="help-center-img img-bordered"/>

***

## Conflict Prevention

GitKraken Desktop’s **Conflict Prevention** helps you detect and manage potential conflicts before they cause disruptions. 

Learn more about [Conflict Prevention →](/gitkraken-desktop/conflict-prevention/)

<div class='callout callout--warning'>
    <p>Conflict Prevention is available for customers on the Advanced tier or higher.</p>
</div>

***

## Rebasing
Rebasing takes the commits from one branch and places them onto the last commit of another branch. This alters the tree structure by moving the commits and their changes onto the target branch.

<div class='embed-container embed-container--16-9'>
<iframe width="560" height="315" src="https://www.youtube.com/embed/xot40u-_1FI" frameborder="0" allowfullscreen></iframe>
</div>

To perform a rebase, drag and drop one branch onto another branch then select <kbd>Rebase</kbd>.

<img src="/wp-content/uploads/select-rebase.png" srcset="/wp-content/uploads/select-rebase@2x.png" class="help-center-img img-bordered">
You can rebase onto a local or remote.

<img src="/wp-content/uploads/select-rebase-sidebar.png" srcset="/wp-content/uploads/select-rebase-sidebar@2x.png" class="help-center-img img-bordered">
Remember, rebasing rewrites history in exchange for a visually cleaner history. 