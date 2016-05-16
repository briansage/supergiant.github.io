[Contrib Guide]: ./source/docs/community/contribution-guidelines.md "Supergiant Community Contribution Guidelines"
[AUTHORS]: /AUTHORS "List of Documentation Authors"
[GitHub Using Pull Requests]: https://help.github.com/articles/using-pull-requests/ "GitHub Help: Using pull requests"

Supergiant Documentation
=======================================================================

This is a central repository for all Supergiant-related documentation. This README you are reading now is about the Documentation repo, itself.

To browse this documentation, see http://supergiant.github.io/, or browse this repo starting at [./source/README.md](./source/README.md)

See below for instructions to run this repo as a GitBook on your own hardware.

This documentation contains references for all relevant Supergiant repositories, their features, how to get started using them, and how to contribute, e.g.

* API reference
* Dashboard UI reference
* Getting started tutorials
* Workflows and concepts
* Code of Conduct
* Contributor License Agreements
* Collaboration Processes
* Etc.


On Collaboration
-----------------------------------------------------------------------

This repo follows the [Community Contribution Guidelines for all Supergiant repositories][Contrib Guide]. Please read our guidelines, and learn how best to contribute. Like good little Zen masters, we think all feedback is helpful, so we welcome contributions from any source, whatever the suggested change.


Host On Your Own
-----------------------------------------------------------------------

We pre-compile every release of this repo as static HTML using GitBook. To host this repo on your own hardware, simply point your web server's `DocumentRoot` or `root` to this project's base directory.


Contribute to Supergiant Documentation
-----------------------------------------------------------------------

To make a contribution to _this_ documentation, please first familiarize yourself with our [Community Contribution Guidelines][Contrib Guide]. When you're ready to get busy, follow these steps:

#### First, become a code contributor

We love that you want to help. Before we can accept your effort, we need you to agree to a Contributor License Agreement. See the Contributor Guidelines section on [How to become a code contributor][Contrib Guide].

#### Second, install dependencies

In order to get going with this repo, you'll need to install, [NodeJS](https://nodejs.org/en/) v4.x or greater, and [GitBook's](https://github.com/GitbookIO/gitbook) CLI tool.


Fork this repository, and then clone it locally. This is they only way you will be able to submit your changes back to GitHub for later inclusion. For example purposes, we'll use this repository URL below.

You will replace this URL with your own fork's URL:

```sh
git clone git@github.com:supergiant/supergiant.github.io.git
```

Install GitBook:

```sh
npm i -g gitbook-cli
```

Run the GitBook server. This may take a while, as additional dependencies may be installed to the local directory for the first time.

```sh
npm run serve
```

#### Then, follow these steps

* Make your changes to the markdown (`.md`) files in the `source/docs` directory.
  All other directories at the root level are automatically generated, so any changes outside of `source/docs` will be overwritten.
* While your local server is running, preview your changes at http://localhost:4000
* Draft your GitBook release: `npm run release`
* Use git to commit and push your changes to a feature branch on your forked repo
* Submit a [Pull Request on GitHub][GitHub Using Pull Requests]

You've contributed, yay! The maintainers will comment on your Pull Request, and they will either ask for changes or accept what you've added. Even if your Pull Request is not accepted immediately, you should feel good about yourself, because any input is valuable for the project.

More detail on these steps, the conduct we expect, and what you can expect from other collaborators can be found in our [Contribution Guidelines][Contrib Guide].


Contributors, Committers, and TC.
-----------------------------------------------------------------------

Everyone involved, on any level, is considered a contributor to the project. Thank you!

If you have at any point added documentation to this repo, we'll add your name to the [Authors list][AUTHORS].


---


[![Analytics](https://ga-beacon.appspot.com/UA-40292794-2/supergiant-documentation/readme)](https://github.com/igrigorik/ga-beacon) What's this?

This is a Google Analytics beacon that allows us to see how many anonymous users are interested in our repositories. In this documentation, this beacon is only placed in the root `README.md`, which is not rendered when this repo is run as a reference GitBook.
