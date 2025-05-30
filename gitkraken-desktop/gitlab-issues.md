---

title: GitKraken Desktop GitLab Issues Integration
description: Learn how to access GitLab Issues from GitKraken Desktop
taxonomy:
    category: gitkraken-desktop

---

<kbd>Last updated: May 2025</kbd>

GitKraken Desktop makes it easy to integrate with GitLab Issues.

<div class='callout callout--basic'>
    <p>The GitHub Issues integration is restricted to Public repositories only for Community users. To unlock all features for the GitHub Issues integration, consider upgrading to a <a href="https://gitkraken.com/pricing?source=help_center&product=gitkraken"> paid GitKraken license</a>. </p>
</div>

***

### Connect GitLab Integration

The GitLab integration and GitLab Issues integration share the same connection. You can Set up the integration from the ISSUES pane in the left panel or from <kbd><i>Preferences   <i class='fa fa-caret-right'></i>   Integrations</i></kbd>.

<img src="/wp-content/uploads/connect-gitlab-issues-2025.png" srcset="/wp-content/uploads/connect-gitlab-issues-2025@2x.png" class="help-center-img img-bordered">


From the Integrations window, select _GitLab.com_ and then hit the <button class='button button--success button--ui button--nolink'>Connect to GitLab</button> button.

<img src="/wp-content/uploads/connect-gitlab-2025.png" srcset="/wp-content/uploads/connect-gitlab-2025@2x.png 2x" class="help-center-img img-bordered">

This will open your default web browser where you can click <button class='button button--success button--ui button--nolink'>Continue authorization</button> and then log in with your GitLab credentials.

<img src="/wp-content/uploads/authorize-gitlab.png" srcset="/wp-content/uploads/authorize-gitlab@2x.png 2x" class="help-center-img img-bordered">

<img src="/wp-content/uploads/gitlab-sign-in.png" srcset="/wp-content/uploads/gitlab-sign-in@2x.png 2x" class="help-center-img img-bordered">

You'll then see a success message below and the connection will be active in GitKraken 🎉

<img src="/wp-content/uploads/auth-success-gitlab-1.png" srcset="/wp-content/uploads/auth-success-gitlab-1@2x.png 2x" class="help-center-img img-bordered">

***

### Preview GitLab Issues

Once connected, your GitLab issues will start to appear in the left panel. You will initally see  _My Issues_ and _All Issues_ filters by default. You can edit or remove these as needed.

<img src="/wp-content/uploads/gitlab-issues-list-2025.png" srcset="/wp-content/uploads/gitlab-issues-list-2025@2x.png" class="help-center-img img-bordered">

Hover over any issue to get a preview of the issue Title, Description, labels, milestones and assignee.

<img src="/wp-content/uploads/gitlab-issue-hover-2025.png" srcset="/wp-content/uploads/gitlab-issue-hover-2025@2x.png" class="help-center-img img-bordered">

***

### View and Edit GitLab Issue Details

Click to select an issue to view the issue details.

<img src="/wp-content/uploads/github-issue-view-click-2025.png" srcset="/wp-content/uploads/github-issue-view-click-2025@2x.png" class="help-center-img img-bordered">

Here any edits made here will be reflected in your GitLab issues.

***

### Create New GitLab Issue

From the left panel, click the <button class='button button--success button--ui button--nolink'>+</button> icon to add a new GitLab issue.

<img src="/wp-content/uploads/gitlab-issue-create-2025.png" srcset="/wp-content/uploads/gitlab-issue-create-2025@2x.png" class="help-center-img img-bordered">

Note that required fields are denoted by `*`. Your new issue will automatically sync with your GitLab issues.

***

### Create Filters

You may create filters to view the issues you need. We use the same syntax that GitLab uses for thier issues.

<img src="/wp-content/uploads/gitlab-filter-create-2025.png" srcset="/wp-content/uploads/gitlab-filter-create-2025@2x.png" class="help-center-img img-bordered">

You can refer to [GitLab issue filtering](https://docs.gitlab.com/ee/user/search/index.html#filtering-issue-and-merge-request-lists) docs from GitLab for more information.

***

### Create Branches from Issue

You may create a branches tied to an issue from the issue details view <button class='button button--success button--ui button--nolink'>Create a branch for this issue</button> button. You can also right-click the issue or click the <kbd> <i class="fa fa-ellipsis-v"></i> </kbd>.

<img src="/wp-content/uploads/gitlab-issue-create-branch-2025.png" srcset="/wp-content/uploads/gitlab-issue-create-branch-2025@2x.png" class="help-center-img img-bordered">

The branch name will automatically prefill based on the issue name. After the branch is created, these branches will be denoted with the GitLab icon to reflect its link to a GitLab issue.

From here, it should be possible to configure triggers on the GitLab side for changes made to this branch.

***

### Copy Issue link or View in GitLab

You can quickly navigate to the issue in GitLab from the <kbd> <i class="fa fa-ellipsis-v"></i> </kbd> menu or by clicking <i class="fa fa-external-link" aria-hidden="true"></i> in the top right.

<img src="/wp-content/uploads/gitlab-issue-copy-link-2025.png" srcset="/wp-content/uploads/gitlab-issue-copy-link-2025@2x.png" class="help-center-img img-bordered">


