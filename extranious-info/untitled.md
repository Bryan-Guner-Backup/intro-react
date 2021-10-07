# About pull request reviews

##

Reviews allow collaborators to comment on the changes proposed in pull requests, approve the changes, or request further changes before the pull request is merged. Repository administrators can require that all pull requests are approved before being merged.

### [In this article](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#in-this-article) <a id="in-this-article"></a>

- [About pull request reviews](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#about-pull-request-reviews)
- [Resolving conversations](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#resolving-conversations)
- [Re-requesting a review](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#re-requesting-a-review)
- [Required reviews](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#required-reviews)
- [Further reading](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#further-reading)

#### [About pull request reviews](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#about-pull-request-reviews) <a id="about-pull-request-reviews"></a>

After a pull request is opened, anyone with _read_ access can review and comment on the changes it proposes. You can also suggest specific changes to lines of code, which the author can apply directly from the pull request. For more information, see "[Reviewing proposed changes in a pull request](https://docs.github.com/en/articles/reviewing-proposed-changes-in-a-pull-request)."

Repository owners and collaborators can request a pull request review from a specific person. Organization members can also request a pull request review from a team with read access to the repository. For more information, see "[Requesting a pull request review](https://docs.github.com/en/articles/requesting-a-pull-request-review)." You can specify a subset of team members to be automatically assigned in the place of the whole team. For more information, see "[Managing code review assignment for your team](https://docs.github.com/en/organizations/organizing-members-into-teams/managing-code-review-assignment-for-your-team)."

Reviews allow for discussion of proposed changes and help ensure that the changes meet the repository's contributing guidelines and other quality standards. You can define which individuals or teams own certain types or areas of code in a CODEOWNERS file. When a pull request modifies code that has a defined owner, that individual or team will automatically be requested as a reviewer. For more information, see "[About code owners](https://docs.github.com/en/articles/about-code-owners)."

You can schedule reminders for pull requests that need to be reviewed. For more information, see "[Managing scheduled reminders for pull requests](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/managing-scheduled-reminders-for-pull-requests)."

![Header of review requesting changes with line comments](https://docs.github.com/assets/images/help/pull_requests/review-header-with-line-comment.png)

A review has three possible statuses:

- **Comment**: Submit general feedback without explicitly approving the changes or requesting additional changes.
- **Approve**: Submit feedback and approve merging the changes proposed in the pull request.
- **Request changes**: Submit feedback that must be addressed before the pull request can be merged.

![Image of review statuses](https://docs.github.com/assets/images/help/pull_requests/pull-request-review-statuses.png)

**Tips**:

- If required reviews are enabled and a collaborator with _write_, _admin_, or _owner_ access to the repository submits a review requesting changes, the pull request cannot be merged until the same collaborator submits another review approving the changes in the pull request.
- Repository owners and administrators can merge a pull request even if it hasn't received an approving review, or if a reviewer who requested changes has left the organization or is unavailable.
- If both required reviews and stale review dismissal are enabled and a code-modifying commit is pushed to the branch of an approved pull request, the approval is dismissed. The pull request must be reviewed and approved again before it can be merged.
- When several open pull requests each have a head branch pointing to the same commit, you won’t be able to merge them if one or both have a pending or rejected review.
- Pull request authors cannot approve their own pull requests.

You can view all of the reviews a pull request has received in the Conversation timeline, and you can see reviews by repository owners and collaborators in the pull request's merge box.

![Image of reviews in a merge box](https://docs.github.com/assets/images/help/pull_requests/merge_box/pr-reviews-in-merge-box.png)

**Tip:** You can find a pull request where you or a team you're a member of is requested for review with the search qualifier `review-requested:[USERNAME]` or `team-review-requested:[TEAMNAME]`. For more information, see "[Searching issues and pull requests](https://docs.github.com/en/articles/searching-issues-and-pull-requests)."

#### [Resolving conversations](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#resolving-conversations) <a id="resolving-conversations"></a>

You can resolve a conversation in a pull request if you opened the pull request or if you have write access to the repository where the pull request was opened.

To indicate that a conversation on the **Files changed** tab is complete, click **Resolve conversation**.

![Pull request conversation with Resolve conversation button](https://docs.github.com/assets/images/help/pull_requests/conversation-with-resolve-button.png)

The entire conversation will be collapsed and marked as resolved, making it easier to find conversations that still need to be addressed.

![Resolved conversation](https://docs.github.com/assets/images/help/pull_requests/resolved-conversation.png)

If the suggestion in a comment is out of your pull request's scope, you can open a new issue that tracks the feedback and links back to the original comment. For more information, see "[Opening an issue from a comment](https://docs.github.com/en/github/managing-your-work-on-github/opening-an-issue-from-a-comment)."

#### [Re-requesting a review](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#re-requesting-a-review) <a id="re-requesting-a-review"></a>

You can re-request a review, for example, after you've made substantial changes to your pull request. To request a fresh review from a reviewer, in the sidebar of the **Conversation** tab, click the icon.

#### [Required reviews](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#required-reviews) <a id="required-reviews"></a>

Repository administrators can require that all pull requests receive a specific number of approving reviews before someone merges the pull request into a protected branch. You can require approving reviews from people with write permissions in the repository or from a designated code owner. For more information, see "[About protected branches](https://docs.github.com/en/github/administering-a-repository/about-protected-branches#require-pull-request-reviews-before-merging)."

**Tip**: If necessary, people with _admin_ or _write_ access to a repository can dismiss a pull request review. For more information, see "[Dismissing a pull request review](https://docs.github.com/en/articles/dismissing-a-pull-request-review)."

#### [Further reading](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-reviews#further-reading) <a id="further-reading"></a>

- "[Reviewing proposed changes in a pull request](https://docs.github.com/en/articles/reviewing-proposed-changes-in-a-pull-request)"
- "[Viewing a pull request review](https://docs.github.com/en/articles/viewing-a-pull-request-review)"
- "[Setting guidelines for repository contributors](https://docs.github.com/en/articles/setting-guidelines-for-repository-contributors)"
