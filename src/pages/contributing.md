---
title: Contributing
---

## Code of Conduct

We want this community to be friendly and respectful to each other. Please read [the full text](./CODE_OF_CONDUCT) so that you can understand what actions will and will not be tolerated.

## Our Development Process

The core team works directly on GitHub and all work is public.

### Development workflow

> **Working on your first pull request?** You can learn how from this *tutorial* : [How to Contribute to an Open Source Project on GitHub](https://egghead.io/series/how-to-contribute-to-an-open-source-project-on-github).

1. Fork the repo and create your branch from `master` (a guide on [how to fork a repository](https://help.github.com/articles/fork-a-repo/)).
2. Run `npm install` to setup the development environment.
3. Do the changes you want and test them before sending a pull request.

### Commit message convention

We follow the [conventional commits specification](https://www.conventionalcommits.org/en) for our commit messages:

* `fix`: bug fixes, e.g. fix Button color on DarkTheme.
* `feat`: new features, e.g. add Snackbar component.
* `refactor`: code refactor, e.g. new folder structure for components.
* `docs`: changes into documentation, e.g. add usage example for Button.
* `test`: adding or updating tests, eg unit, snapshot testing.

### Linting and tests

We use `eslint` for lint the code,  `prettier` for formatting the code, and `jest` for testing. You can also run the following commands manually:

* `npm lint`: format files with `prettier`.
* `npm test`: run unit tests with `jest`.

### Sending a pull request

When you're sending a pull request:

* Prefer small pull requests focused on one change.
* Preview the documentation to make sure it looks good.
* Follow the pull request template when opening a pull request.

When you're working on a component:

* Follow the guidelines described in the [Neumorphism UI Design](https://www.justinmind.com/blog/neumorphism-ui/).
* Write a brief description of every prop when defining `type Props` to aid with documentation.
* Provide an example usage for the component (check other components to get a idea).
* Update the type definitions for Flow if you changed an API or added a component.

### Working on documentation

The documentation is automatically generated from the [Docusaurus](https://docusaurus.io/). To preview the generated documentation, run `npm start` in the project root.

## Reporting issues

You can report issues on our [bug tracker](https://github.com/awaitstack/neumorphism-ui/issues). Please follow the issue template when opening an issue.

## License

By contributing to React Native Neumorphism, you agree that your contributions will be licensed under its **MIT** license.
