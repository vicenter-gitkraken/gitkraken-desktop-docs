---

title: Pull requests
description: Create pull requests directly from GitKraken Desktop and merge one branch into another.
taxonomy:
    category: gitkraken-desktop

---
<kbd>Last updated: April 2025</kbd>

A pull request (sometimes called merge requests), is a review request. You are asking someone to check the changes on a branch before merging into another branch.

<div class='embed-container embed-container--16-9'>
    <iframe width='560' height='315' src='https://www.youtube.com/embed/2VX1ISk9XH8?rel=0&vq=hd1080' frameborder='0' allowfullscreen></iframe>
</div>

***
## Creating a pull request
If connected to a remote on GitHub, GitLab, Bitbucket, or Azure DevOps, create pull requests by dragging and dropping one branch to another and selecting <em class='context-menu'>Start a pull request</em>.

<img src="/wp-content/uploads/create-pull-request-drag-and-drop-2025.gif" class="help-center-img img-bordered">

Alternatively, try right-clicking the target branch and selecting <em class='context-menu'>Start a pull request</em>.

Or click the <button class='button button--success button--ui button--nolink'>+</button> in the pull requests section on the Left Panel, and select the repo and branch to create the pull request.

<img src="/wp-content/uploads/create-pr-2025.png" srcset="/wp-content/uploads/create-pr-2025@2x.png" class="help-center-img img-bordered">

### Pull request templates

GitKraken Desktop supports pull request templates from your GitHub, GitLab, and Azure DevOps (including legacy VSTS URLs).

Once your pull request templates are commited to your remote, the template field will appear when you create a pull request in GitKraken Desktop:

<img src="/wp-content/uploads/pr-template-2025.png" srcset="/wp-content/uploads/pr-template-2025@2x.png" class="help-center-img img-bordered">

A few considerations to keep in mind:
- Verify the appropriate location for your pull request template based on your provider's documentation
- The pull request template must already exist on your currently checked out branch


If this is your first time working with pull request templates, consider reviewing the following instructions for GitHub, GitLab, or Azure DevOps pull request templates.

* [Creating Pull Request templates on GitHub](https://help.github.com/articles/creating-a-pull-request-template-for-your-repository/)

* [Creating Merge Request templates on GitLab](https://docs.gitlab.com/ee/user/project/description_templates.html)

* [Creating Pull Request templates on Azure DevOps](https://docs.microsoft.com/en-us/azure/devops/repos/git/pull-request-templates?view=azure-devops)


### Assignee, Labels, and Reviewers

Some integrations will allow you to also add a pull request assignee(s), reviewer(s) and label(s) to your pull request. GitKraken Desktop will then pass these values onto your remote service when the pull request is created.

<img src='/wp-content/uploads/add-reviewers-assignees-labels-2025.png' srcset='/wp-content/uploads/add-reviewers-assignees-labels-2025@2x.png' class="help-center-img img-bordered">

When creating pull request, GitKraken Desktop detects whether your source branch has conflicts with the target branch in the pull request modal.

<img src='/wp-content/uploads/pr-merge-conflict-warning-2025.png' srcset='/wp-content/uploads/pr-merge-conflict-warning-2025@2x.png' class="help-center-img img-bordered">

<div class='callout callout--basic'>
  <p><strong>Note:</strong> Because pull requests occur in the remote, first push your branch before creating the request.</p>
</div>

### Draft Pull Requests

If connected to the [GitHub Integration](/gitkraken-desktop/github-gitkraken-desktop/), you may create a draft pull request by checking this box when creating a pull request in GitKraken Desktop.

<img src='/wp-content/uploads/create-draft-pr-2025.png' srcset='/wp-content/uploads/create-draft-pr-2025@2x.png' class="help-center-img img-bordered">

As the name implies, this will create a "draft" pull request in GitHub. However please note that not all GitHub free or paid plans support the draft feature. Please check your GitHub plan if you do not see this option.

***

## GitHub pull request view

GitHub.com users may utilize the pull request view for GitHub pull requests.

To enable this feature, first set up the [GitHub integration](/gitkraken-desktop/github-gitkraken-desktop/). Then with a GitHub repo open inside of GitKraken Desktop, select a pull request in the Left Panel (or checkout the source branch and a PR icon with the number shows up next to the branch) to bring up the pull request view. Or from the Launchpad, click on the icon at the right side of the Pull Request.

Repository tab:
<img src='/wp-content/uploads/github-pr-view-2025.png' srcset='/wp-content/uploads/github-pr-view-2025@2x.png' class="help-center-img img-bordered">

Launchpad:

<img src='/wp-content/uploads/launchpad-open-pr-panel-2025.png' srcset='/wp-content/uploads/launchpad-open-pr-panel-2025@2x.png' class="help-center-img img-bordered">

From this view, GitHub users may edit the pull request:

- Title
- Description
- Reviewers
- Assignees
- Milestones
- Labels


From the upper right of the Pull Request view, you may click the <button class='button button--primary button--ui button--nolink'><span style='color:#141422;'>Review Code and Suggest Changes</span></button> button to review the affected files for this pull request. Note, GitHub's code review and GitHub's code comments are not currently available from within GitKraken Desktop.

<img src='/wp-content/uploads/github-pr-review-2025.png' srcset='/wp-content/uploads/github-pr-review-2025@2x.png' class="help-center-img img-bordered">

### Review Code and Suggest Changes

GitKraken has its own native code review, whichs allows you to make suggestions and edits across the entire project in GitKraken Desktop or [gitkraken.dev](https://gitkraken.dev?source=help_center&product=gitkraken). 

With an open Pull Request, you can make suggestions that others can then review and accept.

Open the Pull Request and click on <button class='button button--primary button--ui button--nolink'><span style='color:#141422;'>Review Code and Suggest Changes</span></button>, edit the file, save changes and click on <button class='button button--success button--ui button--nolink'>Suggest X file change to PR #XX </button>

<img src='/wp-content/uploads/gkd-10-2-0-pr-suggest-code-changes.gif' class="help-center-img img-bordered">

### Accept or Reject Code Suggestions

In the GitHub Pull Request panel, you have the ability to review, accept or reject your teammate's code suggestions.
A Pull Request with Code Suggestions has the <em class='context-menu'>Code Suggestions</em> label in it:

<img src='/wp-content/uploads/code-suggestion-2025.png' srcset='/wp-content/uploads/code-suggestion-2025@2x.png' class="help-center-img img-bordered">

Clicking on one of the Code Suggestions opens the repo tab. The Commit Panel shows a diff with the changes so you can review and two options on bottom `Apply suggestion to branch` or `Reject suggestion`.

<img src='/wp-content/uploads/gkc-pr-code-suggestions-apply.gif' class="help-center-img img-bordered">

### Comment on GitHub pull requests
Users may comment on a pull request -- which is great for submitting reviews, approving pull requests, or requesting changes. You may also use the refresh icon in the top right to quickly refresh the comments feed.

<img src='/wp-content/uploads/refresh-comments-2025.png' srcset='/wp-content/uploads/refresh-comments-2025@2x.png' class="help-center-img img-bordered">

You can also quote other comments in your reply from the elipsies <kbd> <i class="fa fa-ellipsis-v"></i> </kbd> menu

<img src='/wp-content/uploads/quote-reply-2025.png' srcset='/wp-content/uploads/quote-reply-2025@2x.png' class="help-center-img img-bordered">

### Branch checkout, build status, and adding remote
If you double-click the branch name in the bottom right of the PR view, GitKraken Desktop will automatically check out the branch and open the graph.

If you click on the build status, GitKraken Desktop will take you to the build URL in your default web browser.

<img src='/wp-content/uploads/build-status-2025.png' srcset='/wp-content/uploads/build-status-2025@2x.png' class="help-center-img img-bordered">

Additionally if you have not added the remote, GitKraken Desktop will ask if you wish to add the remote to the app (which should help you review changes locally).

### Merging within pull request view

GitHub users may also merge a pull request by clicking the <button class='button button--success button--ui button--nolink'>Merge pull request</button> button from within GitKraken Desktop.

<img src='/wp-content/uploads//merge-options.png' srcset='/wp-content/uploads//merge-options@2x.png' class="help-center-img img-bordered">

By default, the merge will default to the <kbd>Create a merge commit</kbd> setting, however you may also choose between <kbd>Squash and merge</kbd> and the <kbd>Rebase and merge</kbd>,

<div class='callout callout--basic'>
  <p>Not seeing something update in the pull request view? Try refreshing GitKraken Desktop to get the latest updates.</p>
</div>


***

## Working with active pull requests

GitKraken Desktop displays active pull requests in your graph with this <em class='context-menu'><img style='height:1.5em;' src='/wp-content/uploads/gk-pull-request-icon.svg'></em> icon. Pull requests also appear in the Left Panel PULL REQUESTS section.

Sections in PULL REQUESTS each denote a filtered view of pull requests on this repository. GitKraken Desktop will start with several pull request filters for you, note the filters such as *My pull requests* and <i>All pull requests</i>. You can modify, delete, or create your own <a href="/working-with-repositories/pull-requests-filter-syntax/">pull request filters</a>.

<img src='/wp-content/uploads/pull-request-icon-and-panel-2025.png' srcset='/wp-content/uploads/pull-request-icon-and-panel-2025@2x.png' class="help-center-img img-bordered">

Quickly search for pull requests using the <i class='fa fa-search'></i>  *Search pull requests* box.

If using the integration with GitHub, GitLab, Azure DevOps, or Bitbucket, you may hover over the pull request in the Left Panel to get a quick view of when the pull request was opened and for which branches.

<img src='/wp-content/uploads//tooltip-general.png' srcset='/wp-content/uploads//tooltip-general@2x.png' class="help-center-img img-bordered">

For the GitLab integration, this tooltip will also show any assignee or labels associated with the pull request.

<img src='/wp-content/uploads//tooltip-gitlab.png' srcset='/wp-content/uploads//tooltip-gitlab@2x.png' class="help-center-img img-bordered">

And for GitHub, this tooltip will show assignees, labels, reviewers, and build status.

<img src='/wp-content/uploads//tooltip-github.png' srcset='/wp-content/uploads//tooltip-github@2x.png' class="help-center-img img-bordered">

Pull requests will be marked with one of the following icons:

 - <i class='fa fa-check' style="color:green"></i> = Continuous Integration checks passed and review(s) have been approved.
 - <i class='fa fa-circle' style="color:orange"></i> = Continuous Integration checks passed or are pending and review(s) have been approved or are pending. (excludes above case where CI has passed and reviews are approved)
 - <i class='fa fa-times' style="color:red"></i> = All other cases, for example Continuous Integration checks failing or review(s) are needed.

Users may also hover the  mouse over each icon to gain quick information about the status.

If the branch changes look good after review, you or a reviewer may merge the branch. However if there are outstanding questions or comments, users can leave a comment on the pull request.

If other changes are required, make the change to your code, and then commit and push to your existing branch. Updating your branch updates the pull request too.
