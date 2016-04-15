# Contributing

Ideally everyone should be comfortable contributing to this repository.  Here are some quick and dirty rules for being a good citizen:

## Atomic commits

One commit should equal one feature or one removable unit of code.  Okay, this is super ambiguous, but just ask yourself this:  If this code breaks in production, how tough is it going to be to prune the commits out and deploy something functional?

## Blog post commit messages

Commit messages should be no longer than 50 characters.  Put details about the commits into a body below the commit message.  Github (and other Git repo management suites) turns these commit messages into nice interfaces to summarize your work.

## Build before any release

```bash
npm run release
```

## Never work on master

All work should be done in feature branches.  Master is the system of truth and where release builds will come from.  Master should never have broken tests, or broken code knowingly merged in.

Squash feature branches and rebase merge to master.  If you have 30 commits on a feature branch, follow this process:

  * `git rebase -i <COMMIT HASH OF FIRST COMMIT BEFORE YOUR BRANCH>`
  * Intelligently pick or squash your 30 commits into as few as possible, ideally 1.
  * Name that commit with 50 characters or less, and write a small blog style post about your changes.
  * `git checkout master && git pull && git checkout - && git rebase master`
  * You are now ready to submit a pull request.  Github will actually turn your blog style commit message into the pull request itself.

## Dependencies

In order to get going with this repo, you'll need to install [Gitbook's](https://github.com/GitbookIO/gitbook) CLI tool:

```bash
npm i -g gitbook-cli
```

Gitbook depends on Node 4+

## Contributors, committers, and TC.

Everyone involved, on any level, is considered a contributor to the project.  Thank you!

If you have at any point added or submitted documentation to this repo, we'll try to add your name to the `authors` entry and a contributors file.
