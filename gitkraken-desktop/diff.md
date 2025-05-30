---

title: Diff, Patch, Blame, and History 
description: Compare your changes with diffs in GitKraken Desktop. Learn about where to access diffs, file blame, and more.
taxonomy:
    category: gitkraken-desktop

---
<kbd>Last updated: April 2025</kbd>

Compare changes within GitKraken Desktop _diffs_. Learn where to access _diffs_, and how to access _file history_ or _file blame_.

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/-0bn2H63axM?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>



***

<a id="what-is-a-diff-in-gitkraken"></a>

## What is a diff in GitKraken Desktop?

A diff shows what was added or removed from a file. <span style='color: #d90171;'>Red</span> is for lines where content was removed whereas <span style='color: #7bd938;'>green</span> is for new lines added.

<img src='/wp-content/uploads/diff-full-screen-2025.png' class="help-center-img img-bordered" />

GitKraken Desktop's diff comes included with the following:

- Word diffing
- Syntax highlighting
- File mini-map
- Toggles between Hunk View, Inline View, and Split View
- Arrows to move between change sets

Most importantly, the <button class="button button--primary button--ui button--nolink"><span style="color:#141422;">Edit in working directory</span></button> button allows you to edit this file directly. Learn more about this feature in [Editing Files](/working-with-files/editing-files) section.

***
## Where can I access the diff?

Access the diff of a file from:

* **Staging**: Click on a file
* **Commit node**: With a commit node selected, click on any file

If you have two commits selected, GitKraken Desktop shows the difference between the two commits.

<img src='/wp-content/uploads/diff-2-commits-2025.png' class="help-center-img img-bordered">

Additionally, select multiple commit rows in the graph using <kbd>Shift</kbd> <kbd>Click</kbd> to show its merged diff:

<img src='/wp-content/uploads/combined-diff-2025.png' class="help-center-img img-bordered">

### Hunk view

Hunk view will show the diff as blocks, without the context of the rest of the file. It's great if you prefer to focus on the change set.

<img src='/wp-content/uploads/hunk-2025.png' class="help-center-img img-bordered" />

### Inline view

Inline view will show the diff within the context of the entire file. 

<img src='/wp-content/uploads/inline-annotated-2025.png' class="help-center-img img-bordered" />

### Split view

Split view will show a side by side diff comparing how the file looked before (left), and how it looks after the change (right). Note, you may select deleted lines with your mouse from split view. 

<img src='/wp-content/uploads/split-2025.png' class="help-center-img img-bordered" />

***

## External diff tools
Configure your preferred external diff tool from <em class='context-menu'>Preferences <i class='fa fa-caret-right'></i> External Tools</em>:

<img src="/wp-content/uploads/external-diff-2025.png" class="help-center-img img-bordered">

GitKraken Desktop currently _only supports_ the following diff tools:

- Beyond Compare
- FileMerge
- Kaleidoscope
- KDiff
- Araxis
- P4Merge

If your diff tool from the list above is installed and is not showing up in the dropdown, then look for an option to install command line tools.

<img src='/wp-content/uploads/beyond-compare.png' srcset='/wp-content/uploads/beyond-compare@2x.png 2x' class='img-bordered center' style="display: block; margin-left: auto; margin-right: auto;" />



If you would like to use another diff tool, navigate to <em class="context-menu">Preferences <i class="fa fa-caret-right"></i> General</em> and set the <kbd>Diff Tool</kbd> to _Git Config Default_. Then open your global `.gitconfig` file and add these additional lines to use that diff tool. Here are some examples for each operating system:

#### Mac OS
```
[diff]
    tool = meld
[difftool "meld"]
    cmd = open -a Meld --args \"$LOCAL\" \"$REMOTE\"
```

#### Linux
```
[diff]
  tool = meld
[difftool "meld"]
  cmd = meld \"$LOCAL\" \"$REMOTE\"
```

#### Windows
```
[diff]
  tool = meld
[difftool]
  prompt = false
[difftool "meld"]
  cmd = meld "$LOCAL" "$REMOTE"
```

***
## Diff multiple commits

Use the <kbd>Shift</kbd> or <kbd>Cmd/Ctrl</kbd> key to select multiple commits in the Commit Graph.

<img src="/wp-content/uploads/select-commits-2025.gif" class="help-center-img img-bordered">

This will produce a combined diff, which lists all files that were added, modified, renamed or deleted between the selected commits in the Commit Panel.

<div class='callout callout--basic'>
    <p><strong>Note:</strong> Are you looking to diff branches? Consider using the <kbd>Cmd/Ctrl</kbd> key to select the head commits of each branch.</p>
</div>

***

## Diff a WIP

When you have a Work in Progress (WIP), you can diff this against any commit or branch by ctrl/command clicking the WIP and then the other desired commit. Alternativley, with your WIP sleected, you can right-click the desired commit or branch and select `Compare commit against working directory`.

<img src='/wp-content/uploads/compare-WIP-2025.png' class="help-center-img img-bordered">

***

## File Blame and History

_File History_ and _File Blame_ information display in the same view.

To access either option, click to view the file diff and the options will appear in the upper right.

<img src='/wp-content/uploads/blame-history-2025.png' class="help-center-img img-bordered">

You may also click on a commit in the graph and then right click a file to access _File History_ or _File Blame_. _File History_ shows that file's commit history on the left.

<img src='/wp-content/uploads/file-history-commit-selected-2025.png' class="help-center-img img-bordered">

_File Blame_ will color code the commit author of each line or hunk.

<img src='/wp-content/uploads/blame-2025.png' class="help-center-img img-bordered">

Use the top toggle button to switch between <kbd>Diff View</kbd>, which shows the selected commit's changes to the file, and the <kbd>File View</kbd>, which shows the file's state at that commit, including the blame info.

## Patch

A patch, or patchfile, is a file describing changes between 2 files. Patch files can be used to distribute changes that a given user would like to make to a particular revision without codifying it onto a git server. Patches can be created from either a commit(s) or a file(s).

### Create patch from file(s)

To create a patch from a commit, right-click a commit and select `Create patch from commit`. You will be prompted to name the patch after.

<img src='/wp-content/uploads/create-patch-2025.png' class="help-center-img img-bordered">

To create a patch from a file, right-click a file and select `Create patch from file changes`. You will be prompted to name the patch after.

<img src='/wp-content/uploads/patch-from-changes-2025.png' class="help-center-img img-bordered">

You can also multi-select files or commits by holding command/ctrl or shift and clicking. You can then right-click the selected files or commits to create a patch from the selected.

<img src='/wp-content/uploads/patch-from-many-files-2025.png' class="help-center-img img-bordered">

### Create patch from Command Palette

Click on the Command Palette icon on the toolbar, or use the keyboard shortcut <kbd>Cmd</kbd>/<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> to launch Command Palette.

<img src="/wp-content/uploads/create-patch-from-command-palette.png" class="help-center-img img-bordered">

### Apply patch from Command Palette

To apply a patch, use the keyboard shortcut `command/ctrl + Shift + P` or click the <i  class="fa fa-magic" style="transform: rotate(225deg)"></i> in the top right of the UI to bring up the Command Palette. Type “Apply Patch" to summon the “Apply Patch” command, and select it to open your file explorer. 

<img src='/wp-content/uploads/apply-patch-2025.png' class="help-center-img img-bordered">

Select your .patch file to then apply changes to your working directory. 


<div class='callout callout--basic'>
    <p>Note: GitKraken Desktop does not yet support generating patches from binary files. This is a preliminary release with better support coming, and if you have feedback please reach out to our <a href="https://www.gitkraken.com/git-client/contact-support?product=gitkraken&source=help_center">support team</a>. </p>
</div>