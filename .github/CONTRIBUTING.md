# Contributing to Stylus

1. [Getting involved](#getting-involved)
2. [How to report issues](#how-to-report-issues)
3. [Adding translations](#adding-translations)
4. [Pull requests](#pull-requests)
5. [Scripts](#scripts)
6. [Updating locale files](#updating-locale-files-admin-only)
7. [Contact us](#contact-us)

## Getting involved

There are a number of ways to get involved with the development of Stylus. Even if you've never contributed to an Open Source project before, we're always looking for help by identifying issues and suggesting improvements.

## How to report issues

When an [**issue**](https://github.com/openstyles/stylus/issues) is opened, a template is provided. Please answer these questions as thoroughly as possible. If we were psychic, we'd be hanging out in casinos playing poker until they kicked us out. We can't read your mind! Please provide step-by-step directions on how to reproduce the issue as well as the versions of your operating system, browser and Stylus.

When adding a **feature request**, please search through the existing issues to see if it the feature has already been requested, added or rejected.

If not, then provide details describing which page the feature will effect, e.g. popup, manager or editor. Then describe the request and explain how you think it would benefit the user experience.


## Adding translations

You can help us translate the extension on [Transifex](https://www.transifex.com/github-7/Stylus).

## Pull requests

* First open an issue to discuss your changes.
* Then download, fork or clone this repository.
<!-- * Use [node.js](https://nodejs.org/) to run `npm install`. -->
* Use the provided `.editorconfig` file with your code editor. Don't know what that is? Then check out https://editorconfig.org/.
* Make any changes within a branch of this repository (not the `master` branch).
* Submit a pull request and include a reference to the initial issue with the discussion.

## Scripts

* `npm run lint` - Run ESLint on all JavaScript files.
* `npm run update` - Runs update-node & update-main scripts.
* `npm run update-quick` - Updates development dependencies (uses `npm update`; does not include new dependencies).
* `npm run update-locales` (admin only)- Updates locale files from Transifex. See the [updating locale files section](#updating-locale-files-admin-only) for more details.
* `npm run update-main` - Runs update-versions & update-codemirror.
* `npm run update-node` - Update development dependencies, removes & reinstalls `node_modules` folder (slow).
* `npm run update-transifex` (admin only) - Upload `en/messages.json` source to Transifex.
* `npm run update-vendor` - Update codemirror, codemirror themes & other vendor libraries.
* `npm run update-versions` - Update version of `manifest.json` to match `package.json`.
* `npm run zip` - Run update-versions, then compress required files into a zip file.

## Updating locale files (admin only)

* Make sure you have the Transifex client installed. Follow the instructions on [this page](https://docs.transifex.com/client/installing-the-client).
* Contact another admin if you need the `.transifexrc` file in the root folder. It includes the API key to use Transifex's API.
* Use `npm run update-locales` in the command line to [update the language files](https://docs.transifex.com/client/pull) in the repo.
* Use `npm run update-transifex` in the command line to [upload the source](https://docs.transifex.com/client/push) `en/messages.json` file to Transifex.

## Contact us

If you prefer a more informal method of getting in touch or starting a conversation, please [join us on Discord](https://discordapp.com/widget?id=379521691774353408) or leave a comment in the [discussion section](https://add0n.com/stylus.html#reviews). We will monitor any discussions there and join in, and it may be a more appropriate venue for opinions and less urgent suggestions.
