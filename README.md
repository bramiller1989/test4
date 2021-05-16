# Repo Template

[![Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/orbitdb/Lobby) [![Matrix](https://img.shields.io/badge/matrix-%23orbitdb%3Apermaweb.io-blue.svg)](https://riot.permaweb.io/#/room/#orbitdb:permaweb.io) [![Discord](https://img.shields.io/discord/475789330380488707?color=blueviolet&label=discord)](https://discord.gg/cscuf5T)

> A template for creating new repositories in the @orbitdb organization

This repository is meant to serve as a general template for how to set up new repositories in the @orbitdb organization. In general, setting up a new repository should take only a few minutes; use this repository as a way of finding example files, and use the following checklist to ensure that you've set up the repository correctly.

## Install

These instructions are basic; you can use any method to do this work. The important part is making sure that you follow the checklist below before publishing the repository.

```sh
# Let's make a new folder
mkdir new-repo && cd new-repo
# Start a Git instance and copy over template files.
git init
cp ../repo-template/* .
# Overwrite this README
mv README.md setup-checklist.md
mv example-README.md README.md
# Go over and check off the checklist, and finally
rm setup-checklist
```

## Checklist

Go through this checklist after creating your repository. It should only take a couple of minutes; if there is a way to make this more efficient, open an issue and let's talk about it here! \m/

### README
- [ ] Copy `example-README.md` from this repository to your directory.
- [ ] Rename all instances of `<Replace Title>` in README to match the new repo title
- [ ] Manually go through and edit the rest of the README.

### Other Files
- [ ] Copy `CODE_OF_CONDUCT.md` verbatim.
- [ ] Should you have a `CHANGELOG.md`?

### Dotfiles
- [ ] Do you need a `.gitignore` file?
- [ ] Do you need an `.npmignore` file?

### GitHub Metadata
- [ ] Have you added a short description to the repository?
  - [ ] Is the description matched in the byline under the title in the README?
- [ ] Have you added topics to the GitHub repository: `orbitdb`, `orbit`, and so on?
  - [ ] Have you added these topics as keywords in the `package.json`?

### `package.json`

- [ ] Is the `author` field correct?
- [ ] Have you added `keywords`?
- [ ] Are the `bugs` and `homepage` fields correct?
- [ ] Have you added tests? Are they matched, here?
- [ ] Have you added a `lint` command, if using [`eslint-config-orbitdb`](https://github.com/orbitdb/eslint-config-orbitdb)?

### Tests

- [ ] Are there automated tests?
- [ ] ...for the browser as well?
- [ ] Are those reflected in CI?
- [ ] Bonus points: Using CircleCI workflows to segment tests?
- [ ] Extra bonus points: Are you cross-testing dependencies (i.e. are changes in `orbit-db-keystore` tested in `orbit-db` as well

### Benchmarks
- [ ] Are there benchmarks?
- [ ] Did you run the benchmarks before / after the change or PR?

### Examples
- [ ] Is there an example folder with usage examples?
- [ ] For the browser as well?

