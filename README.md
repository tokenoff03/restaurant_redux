This repository contains the website configuration and documentation supporting the React Redux website.

## Contents

- [Getting started](#%EF%B8%8F-getting-started)
- [Overview](#-overview)
- [Website configuration](#-website-configuration)
- [Contributing](#-contributing)
- [License](#-license)

## ✈️ Getting started

### Prerequisites

1.  [Git](https://git-scm.com/downloads).
1.  [Node](https://nodejs.org/en/download/) _(version 12 or greater)_.
1.  NPM

### Installation

1.  `cd react-native-website` to go into the project root.
1.  Run `npm` to install the website's workspace dependencies.

### Running locally

1.  `cd website` to go into the website portion of the project.
1.  `npm start` to start the development server _(powered by [Docusaurus](https://v2.docusaurus.io))_.
1.  Open http://localhost:3000/ site in your favorite browser.

## 📖 Overview

### The site was created according to these criteria:
1. Used Functional and Stateful (class-based) components.
2. Manipulated with forms for controlled and uncontrolled components.
3. Method CRUD. Added Search.
4. REST HTTP. API tools (Fetch API, axios, etc.). React API components.
5. Added components for handling API errors.
6. Lifecycle components.
7. Used React Patterns, Pass Functions as data sources. Used Render-function and Implemented Clone element.
8. High-Order-Components.
9. Context API.
10. React Routes.
11. Used React Hooks.
12. Redux
13. Action Dispatch
14. Container Component and Pure Function.
15. connect(), mapDispatchToProps(), mapStateToProps().
16. Manage React UI (User Interface) for Redux BLL (Business Logic Layer)



### Documentation sources

As mentioned above, the `docs` folder contains the source files for docs from "Guides", "Components" and "APIs" tabs on the React Native website (versioned docs).
The doc files for the "Architecture" and "Contribution" tabs are located inside `website` in the respective directories (unversioned/static docs).
In most cases, you will only want to edit the files within those directories.

If you're adding a new doc or you need to alter the order the docs appear in the sidebar, take a look at the `sidebars.json`, `sidebarsArchitecture.json` and `sidebarsContributing.json` files in the `website` directory. The sidebar files contain a list of document ids that should match those defined in the header metadata (aka frontmatter) of the docs markdown files.

### Versioned docs

Part of the React Native website is versioned to allow users to go back and see the Guides or API reference documentation for any given release. A new version of the website is generally generated whenever there is a new React Native release. When this happens, any changes made to the `docs` and `website/sidebars.json` files will be copied over to the corresponding location within `website/versioned_docs` and `website/versioned_sidebars`.

> **_Note:_** Do not edit the auto-generated files within `versioned_docs` or `versioned_sidebars` unless you are sure it is necessary. Edits made to older versions will not be propagated to newer versions of the versioned docs.

Docusaurus keeps track of the list of versions for the site in the `website/versions.json` file. The ordering of versions in this file should be in reverse chronological order.

#### Cutting a new version

1.  `cd react-native-website` to go into the project root.
1.  `cd website` to go into the website portion of the project.
1.  Run `yarn version:cut <newVersion>` where `<newVersion>` is the new version being released.

## 🔧 Website configuration

The main config file for the website can be found at `website/docusaurus.config.js`. This file tells [Docusaurus how to build the website](https://v2.docusaurus.io/docs/configuration). Edits to this file are rarely necessary.

The `core` subdirectory contains JavaScript and React components that are the core part of the website.

The `src/pages` subdirectory contains the React components that make up the non-documentation pages of the site, such as the homepage.

The `src/theme` subdirectory contains the swizzled React components from the Docusaurus theme.

The `showcase.json` file contains the list of users that are highlighted in the React Native showcase.

## 👏 Contributing

### Create a branch

1.  `git checkout main` from any folder in your local `react-native-website` repository.
1.  `git pull origin main` to ensure you have the latest main code.
1.  `git checkout -b the-name-of-my-branch` to create a branch.
    > replace `the-name-of-my-branch` with a suitable name, such as `update-animations-page`

### Make the change

1.  Follow the "[Running locally](#running-locally)" instructions.
1.  Save the files and check in the browser.
1.  Some changes may require a server restart to generate new files. (Pages in `docs` always do!)
1.  Edits to pages in `docs` will only be visible in the latest version of the documentation, called "Next", located under the `docs/next` path.

Visit **http://localhost:3000/docs/next/YOUR-DOCS-PAGE** to see your work.

> Visit http://localhost:3000/versions to see the list of all versions of the docs.

### Test the change

If possible, test any visual changes in all latest versions of the following browsers:

- Chrome and Firefox on the desktop.
- Chrome and Safari on mobile.

### Push it

1.  Run `yarn prettier` and `yarn language:lint` in `./website` directory to ensure your changes are consistent with other files in the repo.
1.  `git add -A && git commit -m "My message"` to stage and commit your changes.
    > replace `My message` with a commit message, such as `Fixed header logo on Android`
1.  `git push my-fork-name the-name-of-my-branch`
1.  Go to the [react-native-website repo](https://github.com/facebook/react-native-website) and you should see recently pushed branches.
1.  Follow GitHub's instructions.
1.  Describe briefly your changes (in case of visual changes, please include screenshots).

## 📄 License

React Native is [MIT licensed](./LICENSE).

React Native documentation is [Creative Commons licensed](./LICENSE-docs).
