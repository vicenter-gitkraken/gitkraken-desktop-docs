---

title: Committing Changes
description: Commit to save your work with GitKraken Desktop easily when changing files.  Learn how to squash, amend and save work when committing.
taxonomy:
    category: gitkraken-desktop

---
<kbd>Last updated: April 2025</kbd>

Commit to save work with GitKraken Desktop when changing files.  Whether you commit to other things in life is up to you...

<div class='embed-container embed-container--16-9'>
    <iframe width='560' height='315' src='https://www.youtube.com/embed/8a6fYPkBDbY?rel=0&vq=hd1080' frameborder='0' allowfullscreen></iframe>
</div>

***

<a id="making-a-commit"></a>

## Making a commit

To make a commit in GitKraken Desktop, select your _Work in Progress_ and to view recent changes on the Commit Panel.

<img src='/wp-content/uploads/select-WIP-2025.png' class="help-center-img img-bordered">

Select the files you wish to stage, and click on any files you wish to review in the diff. To stage all your files, use the keyboard shortcut <kbd>&#8984;</kbd><kbd>Shift</kbd><kbd>S</kbd> for Mac or <kbd>Ctrl</kbd><kbd>Shift</kbd><kbd>S</kbd> for Windows or Linux.

When you’re ready, type your message and hit commit to commit your changes. You can also use this **Commit** keyboard shortcut <kbd>&#8984;</kbd> + <kbd>Enter</kbd> for Mac or <kbd>Ctrl</kbd> + <kbd>Enter</kbd> if you are on Linux or Windows.

<a id="commit-and-push"></a>
### Commit and push

You can commit and automatically push your changes to the remote. Stage changes and type a commit message to enable the option for commit and push.

<img src='/wp-content/uploads/push-after-commit-2025.png' class="help-center-img img-bordered">

The graph updates with your commit, but the undo button or this keyboard shortcut
<kbd>&#8984;</kbd> + <kbd>Z</kbd> for Mac or <kbd>Ctrl</kbd> + <kbd>Z</kbd> for Windows/Linux can undo a commit made by mistake.

<a id="committing-with-co-authors"></a>

### Committing with Co-Authors

To add co-authors to a commit, add a line to your commit description using the following format:
```
    Co-authored-by: INSERT NAME 1 <Email address 1>
    Co-authored-by: INSERT NAME 2 <Email address 2>
    ...and so on

```

<img src='/wp-content/uploads/co-author.png' srcset='/wp-content/uploads/co-author@2x.png 2x' class="help-center-img img-bordered">

The Commit Panel will then show the co-author in the history for that commit:

<img src='/wp-content/uploads/co-author-history.png' srcset='/wp-content/uploads/co-author-history@2x.png 2x' class="help-center-img img-bordered">

### Bypass git hooks

There may be times when you want to skip your Git hooks when making a commit. This can be done on a commit-by-commit basis by selecting the `Skip git hooks` option. 

<div class='callout callout--warning'>
    <p>Note 📝 - Using this option will bypass all hooks that trigger with git commit action.</p>
</div>

<img src='/wp-content/uploads/skip-commits-2025.png' class="help-center-img img-bordered" />

***

<a id="commit-templates"></a>

## Commit Templates

<a id="reading-the-commit-template"></a>

### Reading the Commit Template
When you open a repository, GitKraken Desktop first checks for a commit template set up in your repository's `.git/config`. If no commit template is found, it will then check your default (global) `.gitconfig`. If no commit template is found there either, then no commit template will be populated in GitKraken Desktop.

<a id="creating-and-updating-the-commit-template"></a>

### Creating and Updating the Commit Template
You can create and update a commit template in GitKraken Desktop by visiting <em class='context-menu'>Preferences <i class='fa fa-caret-right'></i> Commit </em> (scroll down in Preferences nav).

<img src='/wp-content/uploads/commit-template-setting-2025.png' class="help-center-img img-bordered">

If a commit template was read from your local git config, any changes you make to the template in GitKraken Desktop will save to the file specified.

If a commit template was not read from your default `.gitconfig` or you are creating a template for the first time, any change you make to the template in GitKraken Desktop will be written to a file called `gkcommittemplate.txt` in your repository's `.git/` directory. GitKraken Desktop will also update your repository's git config `commit.template` setting to point to this file. This allows you to make changes to your local commit template without overwriting your global commit template for all of your other repositories.

#### Commit Template Options

- `Apply this template to commit messages` option will automatically apply the template to the commit message pane.  If this option is not checked, the commit message pane will be blank.

- `Remove comments from commit messages` will remove lines in the template that start with `#` when creating the commit message. 

### Configuring Commit Templates

There are three different ways to set up commit templates in GitKraken Desktop:

* **Create the template in GitKraken Desktop** - This will create a file called `gkcommittemplate.txt` in your repository's `.git/` directory.

* **Add a repo-specific commit template** - Open a terminal in your local repository and run `git config commit.template <path_to_template>`

* **Add a global commit template** - Open a terminal window and run `git config --global commit.template <path_to_template>`
<div class='callout callout--basic'>
    <p> <strong>Note:</strong> Any changes made in GitKraken Desktop to a global commit template will cause GitKraken Desktop to create a `gkcommittemplate.txt` file in your local `.git/` directory and point your repository's git config `commit.template` setting to the `gkcommittemplate.txt` file</p>
</div>


***

<a id="amending-commits"></a>

## Amending commits

GitKraken Desktop allows you to amend a commit message, add additional changes, or both.

To add more changes to the previous commit, first make the code changes in your working directory. Then when you stage changes in GitKraken Desktop, select the option to _"Amend the previous commit."_

<img src='/wp-content/uploads/amend-commit-2025.png' class="help-center-img img-bordered">

To only update the commit message, select the most recent commit in the graph and then click in the message box to amend the message.

<img src='/wp-content/uploads/amend-message-2025.png' class="help-center-img img-bordered">

To accommodate viewing a longer commit description, click on the bar at the the bottom of the message box and drag downwards to dynamically resize the text field.

<img src='/wp-content/uploads/amend-box-2025.png' class="help-center-img img-bordered">

Select <button class='button button--success button--ui button--nolink'>Update Message</button> to save your changes or <button class='button button--danger button--ui button--nolink'>Cancel Amend</button> to discard.

<div class='callout callout--basic'>
    <p><strong>Note:</strong> Amending commits which are already pushed to a remote are more difficult to apply and would require a force push for the rewrite.</p>
</div>

***

<a id="resetting-commits"></a>

## Resetting commits
Git keeps track of your current commit in a file called the HEAD.  When resetting a commit, you update the HEAD of your repo to point to the selected commit.  GitKraken Desktop offers the following reset options:

* **Soft** - resets the HEAD to the selected commit, but keeps your changes staged and in your WIP directory
* **Mixed** - resets the HEAD to the selected commit, unstages your changes, but keeps them in your WIP directory
* **Hard** - resets the HEAD to the selected commit, unstages your changes, and deletes your WIP files

<img src='/wp-content/uploads/reset-commit-2025.png' class="help-center-img img-bordered">

You may also drag and drop a branch onto another to select from the three reset options above or access the reset options from your local repos in the left panel.

***

<a id="reverting-changes"></a>

## Reverting changes

Undo, undo, undo. You can undo many of your actions in GitKraken Desktop with the Undo icon.

<img src='/wp-content/uploads/undo-undo-2025.png' class="help-center-img img-bordered">

If you're a keyboard fan, you may also enjoy using the keyboard shortcut
<kbd>&#8984;</kbd> + <kbd>z</kbd> for Mac or <kbd>Ctrl</kbd> + <kbd>Z</kbd> for not-Mac.

<a id="reverting-commits"></a>

### Reverting commits

Reverting commits is trivial thanks to GitKraken Desktop.

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/U_axv67W1Ik?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>

If you wish to revert a commit (perhaps Undo is not available), the option is available when right-clicking on a commit node.  This will create a new commit to reverse your previous changes.

<img src='/wp-content/uploads/revert-commit-2025.png' class="help-center-img img-bordered">
