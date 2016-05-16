[Contrib Guide]: ./source/docs/community/contribution-guidelines.md "Supergiant Community Contribution Guidelines"
[AUTHORS]: /AUTHORS "List of Documentation Authors"

# Supergiant Documentation

This is a central repository for any Supergiant-related documentation, e.g.

* API reference
* Dashboard UI reference
* Getting started tutorials
* Workflows and concepts
* Collaboration Processes
* Etc.

This guide may be browsed at http://supergiant.github.io/. See below for instructions to run this repo as a GitBook on your own hardware.


## On Collaboration

This repo follows the [Community Contribution Guidelines for all Supergiant repositories][Contrib Guide]. Please read our guidelines, and learn how best to contribute. Like good little Zen masters, we think all feedback is helpful, so we welcome contributions from any source, whatever the suggested change.


## Host On Your Own

We pre-compile every release of this repo as static HTML using GitBook. To host this repo on your own hardware, simply point your web server's `DocumentRoot` to the `/source/_book` directory.


## Contribute to Supergiant Documentation

To make a contribution to _this_ documentation, please first familiarize yourself with our [Community Contribution Guidelines][Contrib Guide]. When you're ready to get busy, follow these steps:

#### First, become a code contributor

We love that you want to help. Before we can accept your effort, we need you to agree to a Contributor License Agreement. See the Contributor Guidelines section on [How to become a code contributor][Contrib Guide].

#### Second, install dependencies

In order to get going with this repo, you'll need to install, [NodeJS](https://nodejs.org/en/) v4.x or greater, and [Gitbook's](https://github.com/GitbookIO/gitbook) CLI tool:

```sh
npm i -g gitbook-cli
```
#### Then, follow these steps

* Fork this repository
* Make your changes
* Draft your GitBook release: `npm run release`
* Commit your changes to a feature branch
* Submit a pull request

You've contributed, yay! The maintainers will comment on your Pull Request, and they will either ask for changes or accept what you've added. Even if your Pull Request is not accepted immediately, you should feel good about yourself, because any input is valuable for the project.

More detail on these steps, the conduct we expect, and what you can expect from other collaborators can be found in our [Contribution Guidelines][Contrib Guide].


## Contributors, Committers, and TC.

Everyone involved, on any level, is considered a contributor to the project. Thank you!

If you have at any point added or submitted documentation to this repo, we'll add your name to the [Authors list][AUTHORS].


---


[![Analytics](https://ga-beacon.appspot.com/UA-40292794-2/supergiant-documentation/readme)](https://github.com/igrigorik/ga-beacon) What's this?

This is a Google Analytics beacon that allows us to see how many anonymous users are interested in our repositories. In this documentation, this beacon is only placed in the root `README.md`, which is not rendered when this repo is run as a reference GitBook.
