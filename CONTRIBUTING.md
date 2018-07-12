# <a href="contributing">Contributing</a>

Thanks for stopping by!

The following sections detail how to contribute to this project in alignment with its goals. Use your best judgement, and don't hesitate to reach out with any questions.

# <a href="table-of-contents">Table of Contents</a>

[**Code of Conduct**](#code-of-conduct)

[**How Can I Contribute?**](#how-can-i-contribute)

* [Reporting Bugs](#reporting-bugs)
* [Requesting Features](#requesting-features)
* [Your First Code Contribution](#your-first-code-contribution)
* [Pull Requests](#pull-requests)

[**Style Guides**](#style-guides)

* [Git Commit Messages](#git-commit-messages)
* [Documentation](#documentation)

[**Additional Notes**](#additional-notes)
* [Label Conventions](#label-conventions)
* [Security Policies](#security-policies)
* [Acknowledgements](#acknowledgements)

# <a href="code-of-conduct">Code of Conduct</a>

This project and all its participants are governed by the [code of conduct](/CODE_OF_CONDUCT.md). All engaging parties are expected to conform to its policies. Please report acts of non-compliance.

# <a href="how-can-i-contribute">How Can I Contribute</a>

## <a href="reporting-bugs">Reporting Bugs</a>

Well, no one is perfect... :hushed: If you find a bug, I want to know about it; let's take care of that sucker!

### Before Submitting A Bug Report

Check the [issue list](https://github.com/TylerJOtte/themes/issues) to see if a respective report already exists. If there's a matching *open* entry, do not open a new issue. Add a comment to the existing issue instead. If there's a matching *closed* entry, open a new issue, and include a link to the closed entry.

### Submitting A Bug Report

**DO NOT** open an issue for security related bugs. Follow the [security policy](#reporting-security-related-bugs) instead. All other bugs are tracked as [GitHub Issues](https://guides.github.com/features/issues/). Open up a new [issue](https://github.com/TylerJOtte/themes/issues), and fill out its containing form in sufficient detail. Thank you for your contribution!

## <a href="requesting-features">Requesting Features</a>

Do you have an idea that will enhance the project? Let me know!

### Before Submitting A Feature Request

Check the [issue list](https://github.com/TylerJOtte/themes/issues) to see if a respective report already exists. If there's a matching *open* entry, do not open a new issue. Add a comment to the existing issue instead. If there's a matching *closed* entry, open a new issue, and include a link to the closed entry.

### Submitting A Feature Request

Feature requests are tracked as [GitHub Issues](https://guides.github.com/features/issues). Open up a new [issue,](https://github.com/TylerJOtte/themes/issues) and fill out its containing form in sufficient detail. Thank you for your contribution!

## <a href="your-first-code-contribution">Your First Code Contribution</a>

Thank you for your interest in contributing to this project! The most helpful  tasks are:

* [Reporting bugs](#reporting-bugs)
* [Requesting features](#requesting-features)
* [Updating documentation](#pull-requests)

### Beginners

New to contributing on GitHub? No problem, we were all new once! Here are are some helpful resources to get you started.

* [First Time Contributors](https://www.firsttimersonly.com)
* [How To Contribute To Open Source Projects](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github)
* [How To Make A Pull Request](http://makeapullrequest.com)
* [GitHub Guides](https://guides.github.com)

## <a href="pull-requests">Pull Requests</a>

Are you interested in updating the documentation? You're in the right spot!

### Examples

* Spelling/grammar changes
* Type corrections, white space, & formatting changes
* Comment clean-up
* Translations
* Missing sections, and/or documentation

### Steps

#### 1) Fork

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

---
#### 2) Branch

As a best practice, perform changes in a local feature branch. Create this branch directly off the `master` branch. Use a descriptive title that starts with the issue # (where 17 is the issue # in example below).

```bash
$ git checkout -b 17-descriptive-branch-title -t upstream/master
```

---
#### 3) Execute

Execute your changes within the local feature branch, and ensure the [documentation style guidelines](#documentation) are followed.

---
#### 4) Commit

As a best practice, keep your changes as logically grouped as possible within individual commits. A Pull Request has no max-commit limit. This also makes it easier for contributors to review commits.

```bash
$ git add my-changed-files
$ git commit
```

Please ensure that your commit messages follow the [commit style guidelines](#git-commit-messages).

If new to contributing, do your best to conform to these guidelines, but don't fret if a mistake occurs. An existing contributor will help course correct it, and the contributor landing the Pull Request will ensure everything follows the project's guidelines.

Please note that multiple commits are often squashed when they're landed.

---
#### 5) Rebase

As a best practice after committing changes, use `git rebase` (not `git merge`) to sync your changes with the primary repo.

  ```bash
$ git fetch upstream
$ git rebase upstream/master
  ```

This ensures that your local feature branch has all the recent changes from `TylerJOtte/themes/master`.

---
#### 6) Push

Once you are certain your commits ready, push your local feature branch to your fork on GitHub.

```bash
$ git push origin 17-descriptive-branch-title
```

---
#### 7) Pull Request

From within GitHub, open up a new Pull Request, and fill out its containing form in sufficient detail. Please include screenshots, and animated GIFs whenever possible. Do not include issue #s in the title. Thank you for your contribution!

---
#### 8) Update

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

---
#### 9) Landing

All Pull Requests are processed through a review and a subsequent approval stage. If the Pull Request is approved, it will then be merged. When it is landed, a comment will be posted to its respective page detailing the commit(s) it landed.

You may notice that GitHub displays the Pull Request as `closed` now. Fret thee not! Review the branch that the Pull Request was raised against (most likely `master`). There's a commit with the name of none other than yours truly on it. :bowtie: Congratulations, and thank you for your contribution!

# <a href="style-guides">Style Guides</a>

## <a href="git-commit-messages">Git Commit Messages</a>

### Subject Line

* Provide a brief description of the change.
* Use the present imperative (e.g., "Fix typo...", not "Fixed typo...").
* Start first word with a capital letter.
* Do not end line with a period.
* Limit to 50 characters or less.
* A properly formed subject can always complete the following statement logically.<br /><br />
  - If applied, this commit will <*your subject line here*>

### Body

* Provide details on what's being changed, and why it's being changed including <br /><br />
  - The way things worked before the change, and what was wrong with that.
  - The way it works now, and why you decided to solve it the way you did.<br /><br />
* Only include how it's being changed if absolutely necessary.
* Do not assume the reviewer is familiar with the original problem.
* Do not assume the code is self-evident or self-documenting.
* Do not include patch-set specific comments.
* Provide one blank line between the subject line and the body.
* Capitalize the start of each paragraph.
* Wrap text to 72 characters or less.
* Bullet points (hyphens or asterisks) can also be used with a hanging indent.

### Last Line

* Include a reference here if your patch fixes an open issue.

  - Use the `Fixes:` with the full URL prefix for bugs.
  - Use the `Refs:` prefix with the full URL for other references.

* Provide one blank line between the body and the reference(s).

### Example

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

## <a href="documentation">Documentation</a>

### General

* Use [Markdown](https://daringfireball.net/projects/markdown/)

### Code Blocks

* Use language-aware fences (e.g., \`\`\`java).
* Use semi-complete code to illustrate the example, not a complete program.
* Use PascalCase for constructor references.
* Use camelCase for instance references.
* Separate operators & operands with spaces between them (e.g., a = b, not a=b).

# <a href="additional-notes">Additional notes</a>

## <a href="label-conventions">Label Conventions</a>

The project's label nomenclature is listed in the tables below. Each issue and Pull Request requires a type, topic, and status label. An entry may have more than one label within a group. If you notice a missing label, please open an issue and submit the recommendation.

### Type

| Label                      | Description                                   |
| -------------------------- | --------------------------------------------- |
| `Type: Bug Report`         | Issue is a confirmed or probable bug.         |
| `Type: Duplicate Entry`    | Issue is already open.                        |
| `Type: Feature Request`    | Issue is a new or updated feature request.    |
| `Type: Invalid Entry`      | Issue is not a valid type (e.g., user error). |
| `Type: Maintenance Report` | Issue is not a bug or a feature request.      |
| `Type: Project Inquiry`    | Issue is a question not of the other types.   |
| `Type: Regression Report`  | Issue is a bug not present in past version.   |

### Topic

| Label                  | Description                                |
| ---------------------- | ------------------------------------------ |
| `Topic: Documentation` | Issue concerns documentation.              |
| `Topic: Linux`         | Issue manifests in a Linux environment.    |
| `Topic: Mac`           | Issue manifests in a Mac OS X environment. |
| `Topic: Windows`       | Issue manifests in a Windows environment.  |

### Status

| Label                    | Description                                    |
| ------------------------ | ---------------------------------------------- |
| `Status: Abandoned`      | Issue will not be addressed at this time.      |
| `Status: Blocked`        | Pull Request for issue stalled by other issue. |
| `Status: Help Wanted`    | Issue needs help from community to solve.      |
| `Status: In Progress`    | Pull Request for issue is being worked on.     |
| `Status: Needs Review`   | Pull Request for issue is ready for review.    |
| `Status: Needs Revision` | Pull Request for issue needs revision.         |

## <a href="security-policies">Security Policies</a>

### Reporting Security-Related Bugs

**DO NOT** open an issue for security related bugs. Instead, email the project maintainer directly at Themes.Security@icloud.com.

#### How do I know if my report contains a security-related bug?

- [ ] Can you access an item that is not yours?
- [ ] Can you access an item that you are not supposed to have access to?
- [ ] Can you access an item that disables a feature for others?

If you answered "yes" to any of the above questions, the report most likely contains a security-related bug. If you answered "no" to all questions, but you're still hesitant, please email the project maintainer directly at Themes.Security@icloud.com.

All bugs are taken seriously; every effort will be made to address your report. Thank you for your contribution!

## <a href="acknowledgements">Acknowledgements</a>

Various sections of this document expand upon content generated by other developers. A grateful high-five to the following for providing great references and guidance.

### Commit Message Guidelines

* [Chris Beams](https://chris.beams.io/posts/git-commit/)
* [Tim Pope](https://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
* [Robert Painsi](https://gist.github.com/robertpainsi/b632364184e70900af4ab688decf6f53)
* [Caleb Thompson](https://robots.thoughtbot.com/5-useful-tips-for-a-better-commit-message)
* [Ran Ziv](https://cwiki.apache.org/confluence/display/ARIATOSCA/Commit+Message+Guidelines)
* [Node.js](https://github.com/nodejs/node/blob/master/doc/guides/contributing/pull-requests.md#the-process-of-making-changes)
* [Ember.js](https://github.com/emberjs/ember.js/blob/master/CONTRIBUTING.md#pull-requests)
* [Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#before-submitting-an-enhancement-suggestion)
* [Nayafia](https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md)

### Labels

* [Dave Lunny](https://medium.com/@dave_lunny/sane-github-labels-c5d2e6004b63)
* [Wagenet](https://github.com/wagenet/StandardIssueLabels)
* [Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#issue-and-pull-request-labels)

### Misc.
* [Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#how-do-i-submit-a-good-enhancement-suggestion)
* [Ember.js](https://github.com/emberjs/ember.js/blob/master/CONTRIBUTING.md#pull-requests)
* [Active Admin](https://github.com/activeadmin/activeadmin/blob/master/CONTRIBUTING.md#1-where-do-i-go-from-here)
* [Nayafia](https://github.com/nayafia/contributing-template/blob/master/CONTRIBUTING-template.md)
* [Node.js](https://github.com/nodejs/node/blob/master/doc/guides/contributing/pull-requests.md#commit-squashing)
* [GitHub Guides](https://guides.github.com)
* [Open Source Guides](https://opensource.guide/how-to-contribute/)
