---

title: Interface Basics
description: Learn the basics of working with the GitKraken Desktop interface.
taxonomy:
    category: gitkraken-desktop

---
<kbd>Last updated: May 2025</kbd>

GitKraken Desktop's UI helps make sense of Git. Below we cover the layout and what the icons represent.

***

From left to right, GitKraken Desktop displays a left reference panel, Commit Graph, and the Commit Panel when working with a repository.

<img src="/wp-content/uploads/interface.png" class="help-center-img img-bordered">


## Toolbar

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Xv9EAJqucOI?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>

In addition to Undo and Redo, the main toolbar houses common repo actions.

<h3>Undo</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-undo-icon.svg' class='img-responsive'></div>
	<div class="flex-item">
		<p>Many actions performed in GitKraken Desktop can be undone. If an action is undoable, the <kbd>Undo</kbd> button will be a solid color ready for action.</p>
	</div>
</div>

<h3>Redo</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-redo-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>What if you undid something, only to realize that you didn't want to undo it? GitKraken Desktop also has a </kbd>Redo</kbd> button so you can undo your undos.</p>
	</div>
</div>


<h3>Pull</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-pull-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>Pull changes from your remote repos with this button. See the <kbd><i class='fa fa-caret-down'></i></kbd> button next to the icon? Click that to customize the type of pull you want to perform:</p>
	</div>
</div>

* Fetch All
* Pull (fast-forward if possible)
* Pull (fast-forward only): equivalent of `git fetch git merge --ff-only` in the CLI
* Pull (rebase): equivalent of `git fetch git rebase` in the CLI

<div class='callout callout--basic'><p><strong>Tip:</strong> If you find yourself repeatedly performing the same pull actions, set the default pull type by clicking the <i class="fa fa-circle"></i> icon to the pull type's left. The default selection will appear as a <i class="fa fa-dot-circle"></i> icon.</p></div>

<h3>Push</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads//gk-new-push-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>Push changes to the remote repo as set in your upstream.</p>
	</div>
</div>

<h3>Branch</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads//gk-new-branch-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>Create a branch on your current local repo.</p>
	</div>
</div>

<h3>Stash</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads//gk-new-stash-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>Stash your work-in-process (<code>// WIP</code>) changes.</p>
	</div>
</div>


<h3>Pop Stash</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads//gk-new-pop-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>Ready to restore your <code>// WIP</code>? Pop that stash and carry on as you were.</p>
	</div>
</div>

<h3>LFS</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads//gk-lfs-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p> Have large files in your repo? This button will appear when you have <a href="/gitkraken-desktop/git-lfs/">LFS</a> enabled on the repository.</p>
	</div>
</div>


<div class='callout callout--basic'><p><strong>Note:</strong> Toggle the toolbar labels by navigating to <kbd><strong>Preferences > UI Preferences</strong></kbd> and toggling the <code>Show toolbar icon labels</code> checkbox.</p></div>

***
## Left Panel

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/4uSXlUUU0ds?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>

Referred to as the Left "ref" Panel, GitKraken Desktop shows the properties below specific to your repository.

* The entire panel and each section can be collapsed or expanded as needed. 
* The panel and each section can be resized by clicking and dragging. 
* Sections can be toggled by right-clicking a section and selecting the desired section from the context menu.
* Sections can be maximized by double-clicking a section header.

<figure class='figure center'>
    <img src='/wp-content/uploads/left-panel-resize-and-collapse.gif' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Resize, collapse, or expand any part of the Left Panel.</figcaption>
</figure>

<h3>Local</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-local-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>References to local branches &mdash; pointers to specific commits allowing work to be separated.</p>
		<p>If you need help with branches, visit our <a href="/working-with-repositories/branching-and-merging">Branching and Merging</a> page.</p>
	</div>
</div>


<h3>Remote</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-remote-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>References to remote branches.</p>
		<p>Set sail into <a href="/working-with-repositories/pushing-and-pulling">pushing and pulling remotes</a> for more.</p>
	</div>
</div>

<h3>Pull Requests</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-pull-requests-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>This shows active requests for merging one branch into another. With the GitHub or Bitbucket integration, new PRs can be created directly from GitKraken Desktop.</p>
		<p>Create your <a href="/working-with-repositories/pull-requests">Pull Request</a> to get your contribution merged.</p>
	</div>
</div>

<h3>Issues</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<i class="fa fa-list-ul fa-3x" aria-hidden="true"></i>
	</div>
	<div class="flex-item">
		<p>Lets you see and work with your issues in GitKraken Desktop</p>
		<p>Hook up to your remote issue tracker of choice - such as <a href="/integrations/jira/">Jira</a>, <a href="/integrations/github-issues/">GitHub</a>, <a href="/integrations/gitlab-issues/">GitLab</a>, or <a href="/integrations/trello/">Trello</a>.</p>
	</div>
</div> 

<h3>Teams</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<i class="fa fa-users fa-3x" aria-hidden="true"></i>
	</div>
	<div class="flex-item">
		<p>Easily see what your <a href="/working-with-repositories/team-view/">Team</a> members are working on.</p>
	</div>
</div>

<h3>Tags</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-tags-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>These represent active pointers to commits but never move. <a href="/working-with-repositories/tags">Tag</a>, you're it!</p>
	</div>
</div>

<h3>Stashes</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads/gk-new-stash-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>Stored file changes in the working copy.</p>
		<p>For saving your loot to play with later, here's more on <a href="/working-with-commits/stashing">stashes</a>.</p>
	</div>
</div>


<h3>Submodules</h3>
<div class="flex-wrap">
	<div class="flex-item">
		<img src='/wp-content/uploads//gk-new-submodules-icon.svg' class='img-responsive'>
	</div>
	<div class="flex-item">
		<p>A Git repository in a subdirectory of the current repository.</p>
		<p>Git-inception with <a href="/working-with-repositories/submodules">submodules</a> anyone?</p>
	</div>
</div>


***

## Commit Panel

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/ujgcCLBQvm0?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>

The Commit Panel is where files and changes from your working directory are staged and committed.

<figure class='figure center'>
    <img src='/wp-content/uploads/commit-graph-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Previously known as the right panel, the Commit Panel shows file changes and commit details.</figcaption>
</figure>

The three parts in order of operations on the staging panel are:

1. _Unstaged Files_ &mdash; Watched files in your working directory that have changed since the last commit.
 *  Renamed, deleted, new, or modified files appear here.
2. _Staged Files_ &mdash; Files manually added to the index that are ready to commit.
 * Individual lines, hunks, or all of the changes can be added
3. _Commit Message_ &mdash; recording staged changes to the repository
 * Summary: The brief but meaningful message supporting your commit.  This text will appear in the graph.
 * Description: The extended message to provide more details behind the changes.

 Also, here is a quick color guide for the file symbols:

 <figure class='figure center'>
    <img src='/wp-content/uploads/color-guide-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Reference guide for different types of file changes.</figcaption>
</figure>


For deeper waters on staging, dive into [committing work](/working-with-commits/commits).

***
## Commit Graph

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/YWGpKPMALOs?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>

Oooo <span style='color: #0669f7;'>c</span><span style='color: #8e00c2;'>o</span><span style='color: #c517b6;'>l</span><span style='color: #d90171;'>o</span><span style='color: #f25d2e;'>r</span><span style='color: #7bd938;'>s</span>!

<figure class='figure center'>
    <img src='/wp-content/uploads/commit-graph-adjust-2025.gif' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Drag and drop to resize the Commit Graph.</figcaption>
</figure>

The **Commit Graph** in GitKraken Desktop is the core of your repo and a representation of the [Directed Acyclic Graph](https://en.wikipedia.org/wiki/Directed_acyclic_graph) (DAG).  Your commits are displayed here, along with commits from other contributors.

Each row of the graph represents one commit, and the top is always for the latest changes. An interactive _//WIP_ (Work-In-Progress) node will show if the working directory has changed since the last commit.

Branches and tag labels on the left side of the graph are pointers to specific commits, and each vertical column represents a branch currently available on the repository.

Columns can intersect through merge commits as shown in the graph legend. As also shown, multiple branches can be at the same place of a single commit and can be both local and remote.

<figure class='figure center'>
    <img src='/wp-content/uploads/graph-elements.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Use this as a guide for interpreting your commit history in GitKraken Desktop.</figcaption>
</figure>

For a given vertical track, you can read from bottom to top, and right to left to see how changes are introduced into a focused branch.

### Ghost branches

Hover over a commit to view the "ghost" branch, which is the closest branch that contains that commit. The “ghost” branch will also show when a commit is selected, and double-clicking that ghost branch will checkout the head of the referenced branch.


<figure class='figure center'>
    <img src="/wp-content/uploads/ghost.gif" class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Note the branches that appear on the left side of the figure with each mouse action.</figcaption>
</figure>

### Commit highlighting

When you hover over a branch, the app will highlight all commits referenced by that branch.

<figure class='figure center'>
    <img src="/wp-content/uploads/Commit-highlight.png" class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Note how unrelated commits fade when you hover over a branch.</figcaption>
</figure>

Users may toggle this setting on or off from <kbd>Preferences > UI Customization</kbd>.

***

## Tabs

<div class='embed-container embed-container--16-9'>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/QWmjobrj0Qw?ecver=1" frameborder="0" allowfullscreen></iframe>
</div>

***

Quickly switch between multiple repositories.

<figure class='figure center'>
    <img src='/wp-content/uploads/tabs-2025.gif' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Rearrange the tab order with a drag and drop.</figcaption>
</figure>

You can  add new tabs, drag & drop to rearrange, and remove tabs from the top bar. You can also use the corresponding shortcut keys <kbd>cmd</kbd>+<kbd>1-9</kbd> on Windows/Linux and <kbd>cmd</kbd>+<kbd>1-9</kbd> on mac to quickly switch between repositories.

<div class='callout callout--success'>
    <p><b>Tip:</b> You can <b>open</b> a new tab with the <kbd>+</kbd> icon (shortcut: <kbd>cmd/ctrl</kbd>+<kbd>T</kbd>) and you can <b>close</b> a tab with middle-click (shortcut: <kbd>cmd/ctrl</kbd>+<kbd>W</kbd>)  </a></p>
</div>


Tabs are saved for each profile, so you can have multiple sets of tabs that will open when you switch [profiles](/start-here/profiles/)!

<figure class='figure center'>
    <img src='/wp-content/uploads/profile-tabs-2025.gif' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Note how the tabs automatically change when switching profiles.</figcaption>
</figure>

Access a list of all open repositories from the arrow drop-down.

<figure class='figure center'>
    <img src='/wp-content/uploads/tab-drop-down-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">See all open tabs from this carrot icon.</figcaption>
</figure>

Hover over an open tab to quickly see the end portion of the file path.

<figure class='figure center'>
    <img src='/wp-content/uploads/tab-hover-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Get path information when you hover over a tab.</figcaption>
</figure>

### Tab alias and name

An alias can be set for repository tabs. To give an alias to a repository tab, right-click the tab and select <kbd>Alias reposiotry</kbd>. After filling out the name, select save.

<figure class='figure center'>
    <img src='/wp-content/uploads/repository-alias.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Right-click a tab to set a different name.</figcaption>
</figure>



***

## Columns

GitKraken Desktop will show 3 columns in the header by default: <kbd>Branch/Tag</kbd>, <kbd>Graph</kbd>, and <kbd>Commit Message</kbd>. These 3 columns are dynamic and can be rearranged with a drag-and-drop.

<figure class='figure center'>
    <img src='/wp-content/uploads/columns-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Rearrange the column order by drag and drop.</figcaption>
</figure>


Right-click on any column header to enable or disable additional columns such as <kbd>Commit Author</kbd>, <kbd>Commit Date/Time</kbd>, or <kbd>Sha</kbd>. 

<figure class='figure center'>
    <img src='/wp-content/uploads/customize-columns-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Toggle which columns to show or hide from any header.</figcaption>
</figure>

Alternatively, click the <i class="fas fa-cog"></i> icon to enable or disable columns like Branch/Tag, Graph, Commit Message, Author, Date/Time, Sha, or change to Compact Graph view. 

<figure class='figure center'>
    <img src='/wp-content/uploads/gear-2025.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Get the same toggle menu from the gear icon.</figcaption>
</figure>


In addition to using <kbd>cmd/ctrl</kbd>+<kbd>F</kbd> to search commits, users may also filter by commit author. Click the <i class='fa fa-filter'></i>  icon in the AUTHOR column and you can:

- Select one or more users from the drop-down
- Select one or more teams which will filter by all users in that team
- Search for teams or users in the search field

<figure class='figure center'>
    <img src='/wp-content/uploads/filter-author@2x.png' class="help-center-img img-bordered">
    <figcaption style="text-align: center; color: #888;">Type the name of an author or team to filter the Commit Graph.</figcaption>
</figure>

Columns may also be toggled from <kbd><strong>Preferences > UI Customization</strong></kbd>, GitKraken Desktop will remember which columns you have selected, column size, and orientation for each repo. 

For more details on the interface, like soloing remotes, visit [Hiding and Soloing](/working-with-repositories/hiding-and-soloing).
