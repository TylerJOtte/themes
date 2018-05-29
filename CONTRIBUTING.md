
# Contributing

Thanks for stopping by!

The following is a set of guidelines on how to contribute to this project in alignment with its goals. Use your best judgement, and don't hesitate to reach out with any questions.


## Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [How Can I Contribute?](#how-can-i-contribute)
  * [Reporting Bugs](#reporting-bugs)
  * [Requesting Features](#requesting-features)
  * [Your First Code Contribution](#your-first-code-contribution)
  * [Pull Requests](#pull-requests)
3. [Style Guides](#style-guides)
  * [Git Commit Messages Style Guidelines](#git-commit-message-style-guidelines)
  * [Documentation Style Guidelines](#documentation-style-guidelines)
4. [Additional Notes](#additional-notes)
  * [Issue & Pull Request Labels](#issue-&-pull-request-labels)

---
### Code of Conduct
---

This project and all its participants are governed by the [code of conduct](/CODE_OF_CONDUCT.md). All engaging parties are expected to conform to the policies contained within it. Please report acts in non-compliance of the code's stated standards.

---
### How Can I Contribute
---

#### Reporting Bugs

Well, no one is perfect... :hushed: If you find a bug, I want to know about it; let's take care of that sucker!

##### Before Submitting A Bug Report

Check the [issue list](https://github.com/TylerJOtte/themes/issues) to see if a respective report already exists. If there's a matching *open* entry, do not open a new issue. Add a comment to the existing issue instead. If there's a matching *closed* entry, open a new issue, and include a link to the closed entry.

##### Submitting A Bug Report

**DO NOT** open an issue for security related bugs. Follow the [security policy](#security) instead. All other bugs are tracked as [GitHub Issues](https://guides.github.com/features/issues/). Open up a new [issue]((https://github.com/TylerJOtte/themes/issues), and fill out its containing form in sufficient detail. Thank you for your contribution!

#### Requesting Features

Do you have an idea that will enhance the project? Let me know!

##### Before Submitting A Feature Request

Check the [issue list](https://github.com/TylerJOtte/themes/issues) to see if a respective report already exists. If there's a matching *open* entry, do not open a new issue. Add a comment to the existing issue instead. If there's a matching *closed* entry, open a new issue, and include a link to the closed entry.

##### Submitting A Feature Request

Feature requests are tracked as [GitHub Issues](https://guides.github.com/features/issues). Open up a new [issue,]((https://github.com/TylerJOtte/themes/issues) and fill out its containing form in sufficient detail. Thank you for your contribution!

#### Your First Code Contribution

Thank you for your interest in contributing to this project! The most helpful  tasks are:

* [Reporting bugs](#bug-reports)
* [Requesting features](#feature-requests)
* [Updating documentation](#pull-requests)

**Note**: Please do not submit new color themes. This is outside the project's goal. Instead, clone and modify to your heart's delight!

##### Beginners

New to contributing on GitHub? No problem, we were all new once! Here are are some helpful resources to get you started.

* [First Time Contributors](https://www.firsttimersonly.com)
* [How To Contribute To Open Source Projects](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github)
* [How To Make A Pull Request](http://makeapullrequest.com)
* [GitHub Guides](https://guides.github.com)

#### Pull Requests

Are you interested in updating the documentation? You're in the right spot!

##### Examples

* Spelling/grammar changes
* Type corrections, white space, & formatting changes
* Comment clean-up
* Translations
* Missing sections, and/or documentation

##### Steps

###### 1) Fork

[Fork](https://help.github.com/articles/fork-a-repo/) the [project](https://github.com/TylerJOtte/themes) on GitHub. Then, clone your fork locally.

```bash
$ git clone git@github.com:username/themes.git
$ cd themes
$ git remote add upstream https://github.com/TylerJOtte/themes.git
$ git fetch upstream
```

Ensure that your git identity is configured locally.

```bash
$ git config user.username
$ git config user.email
```

If an empty prompt or incorrect information results, set up a proper identity.

```bash
$ git config user.username "username"
$ git config user.email "username@domain.com"
```

Lastly, verify that your [GitHub email list](https://github.com/settings/emails) contains this local email. This enables your commits to properly associate with your account, resulting in a promotion to *Contributor* after your first commit executes.

###### 2) Branch

As a best practice, perform changes in a local feature branch. Create this branch directly off the `master` branch. Use a descriptive title that starts with the issue # (where 17 is the issue # in example below).

```bash
$ git checkout -b 17-descriptive-branch-title -t upstream/master
```

###### 3) Execute

Execute your changes within the local feature branch, and ensure the [documentation style guidelines](#documentation-style-guide) are followed.

###### 4) Commit

As a best practice, keep your changes as logically grouped as possible within individual commits. A Pull Request has no max-commit limit. This also makes it easier for contributors to review commits.

```bash
$ git add my-changed-files
$ git commit
```

Please ensure that your commit messages follow the [commit style guidelines](#commit-style-guide).

If new to contributing, do your best to conform to these guidelines, but don't fret if a mistake occurs. An existing contributor will help course correct it, and the contributor landing the Pull Request will ensure everything follows the project's guidelines.

Please note that multiple commits are often [squashed](#commit-squashing) when they're landed.

###### 5) Rebase

As a best practice after committing changes, use `git rebase` (not `git merge`) to sync your changes with the primary repo.

  ```bash
$ git fetch upstream
$ git rebase upstream/master
  ```

This ensures that your local feature branch has all the recent changes from `TylerJOtte/themes/master`.

###### 6) Push

Once you are certain your commits ready, push your local feature branch to your fork on GitHub.

```bash
$ git push origin 17-descriptive-branch-title
```

###### 7) Pull Request

From within GitHub, open up a new Pull Request, and fill out its containing form in sufficient detail. Please include screenshots, and animated GIFs whenever possible. Do not include issue #s in the title. Thank you for your contribution!

###### 8) Update

You will most likely receive feedback and/or change requests to your Pull Request. Don't be discouraged by this! Some Pull Requests are approved immediately, while others require further discussion. This is a vital step to ensure that changes are necessary and correct.

If you are prompted to make changes to an existing Pull Request, make the changes in your local feature branch, and create a new commit with those changes.

```bash
$ git add my-changed-files
$ git commit
```

Ensure that your branch is synchronized with other changes that have landed in `master`, and then push your branch to your fork. GitHub will then automatically update the Pull Request.

```bash
$ git fetch --all
$ git rebase origin master
$ git push --force-with-lease origin 17-descriptive-branch title
```

**IMPORTANT**: The `git push --force-with-lease` command is one of the few commands in `git` that can delete history. Ensure that you understand the risks before executing it. If uncertain, don't hesitate to ask for guidance in the Pull Request.

Don't worry if you accidentally made a mistake in a commit. For example, you can amend the last commit message.

```bash
$ git add my-changed-files
$ git commit --amend
$ git push --force-with-lease origin feature/branch
```

###### 9) Landing

All Pull Requests are processed through a review and a subsequent approval stage. If the Pull Request is approved, it will then be merged. When it is landed, a comment will be posted to its respective page detailing the commit(s) it landed.

You may notice that GitHub displays the Pull Request as `closed` now. Fret thee not! Review the branch that the Pull Request was raised against (most likely `master`). There is commit with the name of none other than yours truly on it. :bowtie: Congratulations, and thank you for your contribution!

---
### Style Guides
---

#### Git Commit Messages Style Guidelines

###### Subject Line

* Provide a brief description of the change.
* Use the present imperative (e.g., "Fix typo...", not "Fixed typo...").
* Start first word with a capital letter.
* Do not end line with a period.
* Limit to 50 characters or less.
* A properly formed subject can always complete the following statement logically. <br /><br />
 > If applied, this commit will <*your subject line here*>

###### Body

* Provide details on what's being changed, and why it's being changed including

  - The way things worked before the change, and what was wrong with that.
  - The way it works now, and why you decided to solve it the way you did. <br /><br />
* Only include how it's being changed if absolutely necessary.
* Do not assume the reviewer is familiar with the original problem.
* Do not assume the code is self-evident or self-documenting.
* Do not include patch-set specific comments.
* Provide one blank line between the subject line and the body.
* Capitalize the start of each paragraph.
* Wrap text to 72 characters or less.
* Bullet points (hyphens or asterisks) can also be used with a hanging indent.

###### Last Line

* Include a reference here if your patch fixes an open issue.

  - Use the `Fixes:` with the full URL prefix for bugs.
  - Use the `Refs:` prefix with the full URL for other references.

* Provide one blank line between the body and the reference(s).

###### Example

```text
Subject line explains change in <= 50 characters

Body elaborates on the change, if necessary. Keep it wrapped to 72
characters or less. The blank line between the subject line and the body
is vital, unless the body is omitted altogether. Tools, such as rebase,
can become confused if execute the two sections together.

Use the present imperative for the subject line. For example, write "Fix
bug" instead of "Fixed bug". This provides consistent formatting with
commit messages produced by git commands, such as git merge and git
revert. Every additional paragraph is separated by a blank line.

- Bullet points (hyphens or asterisks) can also be used
- Use a hanging indent  

Fixes: https://github.com/TylerJOtte/themes/issues/17
Refs: https://github.com/HappenApps/Quiver/wiki
```
#### Documentation Style Guidelines

###### General

* Use [Markdown](https://daringfireball.net/projects/markdown/)

###### Code Blocks

* Use language-aware fences (e.g., \`\`\`java).
* Use semi-complete code to illustrate the example, not a complete program.
* Use PascalCase for constructor references.
* Use camelCase for instance references.
* Separate operators & operands with spaces between them (e.g., a = b, not a=b).

---
### Additional notes
---

#### Issue & Pull Request Labels
