# Style Guide

## Introduction

This styleguide was created for personal reference, fell free to clone this repo and use it on your own projects. The purpose of this styleguide is to provide more readable and consistent git commits in your projects.

## Commit Messages

### Message Structure

The commit message consists of three distinct parts separated by a blank line: the title, an optional body and an optional footer. Should look something like this:

``` text
type: subject

body

footer
```

#### The title

Consists of the type of message and subject.

#### The Type

The type is contained within the title and can be one of these types:

* **Feat**: a new feature
* **Edit**: any change to the code aside from new feature or code formatting;
* **Fix**: a bug fix
* **Docs**: changes to documentation
* **Format**: code formatting, missing semi colons, etc; no code change
* **Refactor**: refactoring production code, functions, loops, etc
* **Test**: adding tests, refactoring test; no production code change
* **Chore**: updating build tasks, package manager configs, etc; no production code change

#### The Subject

Subjects should be no greater than 50 characters, should begin with a capital letter and do not end with a period.

Use an imperative tone to describe what a commit does, rather than what it did. For example, use change; not changed or changes. Add; not added, etc.

#### The Body

Not all commits are complex enough to warrant a body, therefore it is optional and only used when a commit requires a bit of explanation and context. Use the body to explain the what and why of a commit, not the how.

When writing a body, the blank line between the title and the body is required and you should limit the length of each line to no more than 72 characters.

#### The Footer

The footer is optional and is used to reference issue tracker IDs.

### Example Commit Message

#### Terminal

``` text
git commit -m "feat: Summarize changes in..." -m "More detailed explanatory text, if necessary. Wrap it to about 72characters or so. In some contexts, the first line is treated.." -m "Explain the problem that this commit is solving. Focus on why you are making this change as opposed to how..." -m "- Bullet points are okay too" -m "If you use an issue tracker, put ref..." -m "Resolves: #123" -m "See also: #456"
```

``` text
feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequenses of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```