This repository contains the website configuration and documentation supporting the React Redux website.

## Contents

- [Getting started](#%EF%B8%8F-getting-started)
- [Overview](#-overview)
- [Screenshots](#👏-Screenshots)


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

## 👏 Screenshots
### WelcomePage:

<p align="center">
 <img width="600" src="public/assets/index.png" alt="welcome"/>
</p>

### MenuPage:
Using API we took data
<br>
<p align="center">
 <img width="600" src="public/assets/menu.png" alt="welcome"/>
</p>

### Searching:

props.array.include() function was used
<br>
<p align="center">
 <img width="600" src="public/assets/search.png" alt="welcome"/>
</p>

### Description Page:
We took the menu by id in the request parameter

<br>
<p align="center">
 <img width="600" src="public/assets/desc.png" alt="welcome"/>
</p>

### Reviews Page:
In this page we use CRUD. Used Redux BLL (Business Logic Layer)

<br>
<p align="center">
 <img width="600" src="public/assets/reviews.png" alt="welcome"/>
</p>
