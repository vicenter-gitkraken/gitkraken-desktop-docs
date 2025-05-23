---

title: Staging
description: Learn how to stage and review your files before making your commit.
taxonomy:
    category: gitkraken-desktop

---
<kbd>Last updated: April 2025</kbd>

Staging changes is a breeze with GitKraken Desktop. Let's show you how it works!

***

<a name="staging-files"></a>

## Staging files

Staging adds selected file contents to the index, which is like flagging your work as good to go.
To start, select the _//WIP_ node from the Commit Graph to see all your changes in the Commit Panel.

<img src='/wp-content/uploads/select-WIP-2025.png' class="help-center-img img-bordered">

Once the //WIP node is selected, a <button class='button button--success button--ui button--nolink'>Stage File</span></button> will appear when you hover over a file in the Commit Panel.

<img src='/wp-content/uploads/stage-file-2025.png' srcset="/wp-content/uploads/stage-file-2025@2x.png" class="help-center-img img-bordered">

Additionally, you may click on a file for review in the diff or click the <button class='button button--success button--ui button--nolink'>Stage all changes</span></button>. To stage specific lines, select the file, highlight the target lines, then right-click to access the <em>Stage selected lines</em> option.

<img src='/wp-content/uploads/stage-selected-lines-2025.png' class="help-center-img img-bordered">

<div class='callout callout--success'>
    <p>For quick staging, check out the available <a href="/gitkraken-desktop/keyboard-shortcuts/#repo-actions">Staging Keyboard Shortcuts</a> on hand!</p>
</div>

From here you should be set to  <a href="/gitkraken-desktop/commits">commit</a>!

<a name="unstaging"></a>

### Unstaging

Unstage files by selecting a staged file and hitting the <button class='button button--danger button--ui button--nolink'>Unstage File</span></button> button that appears. 

<img src='/wp-content/uploads/unstage-file-2025.png' srcset="/wp-content/uploads/unstage-file-2025@2x.png" class="help-center-img img-bordered">

If you click on a file to view the diff, you can selectively unstage lines or hunks.

<img src='/wp-content/uploads/unstage-hunk-2025.png' class="help-center-img img-bordered">

If you need to unstage all files, use the <button class='button button--danger button--ui button--nolink'>Unstage all changes</button> button just above the Staged Files section. From here you should be set to <a href="/gitkraken-desktop/commits">commit</a>!

***

<a name="discarding-files"></a>

## Discarding files

As you review your files, you may meticulously stage lines or hunks of changes or discard changes.

<img src='/wp-content/uploads/discard-line-hunk.gif' srcset='/wp-content/uploads/discard-line-hunk@2x.gif' class="help-center-img img-bordered">

To discard changes, select the _//WIP_ node to summon the <i class="fa fa-trash-o" aria-hidden="true"></i> icon. This option will discard all changes or discard any multi-selected files.

<img src='/wp-content/uploads/discard-all-changes-2025.png' srcset="/wp-content/uploads/discard-all-changes-2025@2x.png"  class="help-center-img img-bordered">

To discard a specific group of changes, multi-select files and then right-click to **multi-discard**, or click the <i class="fa fa-trash-o" aria-hidden="true"></i> icon.

<img src='/wp-content/uploads/multi-discard-2025.png' srcset="/wp-content/uploads/multi-discard-2025@2x.png" class="help-center-img img-bordered">

Next, you may discard hunks of changes from the  <a href="/gitkraken-desktop/diff">diff</a> of any file.

<img src='/wp-content/uploads/discard-hunk-ex-2025.png' class="help-center-img img-bordered">

Alternatively in the staging panel, `Discard Changes` is available in the context menu by right-click.

***

<a name="ignoring-files"></a>

## Ignoring Files

You can use the `.gitignore` file to tell GitKraken Desktop to ignore files in your repo that you don't want to be tracked.  

Refer to the `.gitignore` documentation for rules and formatting on the  <a href="https://git-scm.com/docs/gitignore">git-scm website</a>.

To ignore a file, right click on the file in the Commit Panel and select Ignore.

<img src='/wp-content/uploads/ignore-file.png' srcset='/wp-content/uploads/ignore-file@2x.png 2x' class="help-center-img img-bordered">

From this menu you may choose to ignore:
 * The specific file selected
 * All files with that same file extension
 * All files in that same directory 

GitKraken Desktop will create the `.gitignore` file (unless one already exists) at the root of your repo directory and add the appropriate entry, based on your ignore selection.  

<div class='callout callout--note'>
    <p><strong>Note:</strong> GitKraken Desktop will only look at the <code>.gitignore</code> located at the root of your repo directory.  Nested .gitignore files are not parsed.</p>
</div>

<a name="ignoring-previously-tracked-files"></a>

### Ignoring previously tracked files

If a file was previously committed to your repo, then you will see the following options when you attempt to ignore it:

<img src='/wp-content/uploads/ignore-stop-tracking-2025.png' class="help-center-img img-bordered">

Selecting `Ignore` will add the corresponding entry to the `.gitignore file`, but the changes will not be ignored, because the file is already being tracked by Git. 

<img src='/wp-content/uploads/ignore-only.png' srcset='/wp-content/uploads/ignore-only@2x.png' class="help-center-img img-bordered">

Selecting `Ignore and Stop Tracking` will add the corresponding entry to the `.gitignore` file and remove the file from the Git index, so Git stops tracking it.

<img src='/wp-content/uploads/ignore-untrack.png' srcset='/wp-content/uploads/ignore-untrack@2x.png' class="help-center-img img-bordered">
