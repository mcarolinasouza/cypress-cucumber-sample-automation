
[![Cypress.io](https://img.shields.io/badge/tested%20with-Cypress-04C38E.svg)](https://www.cypress.io/)

This project main goal is to build up an automation and consolidate learning about cypress based on the course "Testes de aplicações modernas com Cypress" by Francisco Wagner Costa Aquino.
The other goal is construct a project using Cypress, Cucumber frameworks and BDD concepts.

It is a functional end-to-end automation

## Project structure

```
├── cypress
│   ├── config
│   │   └── data.json
│   ├── fixtures
│   │   └── data.json
│   ├── integration
│   │   └── Conta.feature
│   ├── plugins
│   │   └── index.js
│   └── support
│       ├── pageObjects
│       │   ├── accountPage.js
│       │   ├── loginPage.js
│       │   └── transitionPage.js
│       ├── steps
│       │   ├── accountSteps.js
│       │   └── transitionSteps.js
│       ├── commands.js
│       └── index.js
├── node_modules
├── README.md
├── cypress.json
├── package-lock.json
└── package.json
```

- config - Environment

- fixtures - Test Data

- integration - Tests

- plugins - Events Listeners

- support - Reusable scripts and page objects

- node_modules - Modules for Cypress

- cypress.json - Cypress Configuration

- package.json Dependencies for Cypress

## Local execution

This section will help you to run automation tests based on our project. Follow these steps to run:

    1. Clone automation project in your local machine
    2. Open your VSCode terminal and go to cloned folder
    3. Ensure you are on root folder of project (folder that has package.json)
    4. Go to the "Installing" section of this tutorial, and follow the steps
    5. Go to the "Running Tests" section of this tutorial, and follow the steps
## Installing

[![npm version](https://d25lcipzij17d.cloudfront.net/badge.svg?id=js&r=r&type=6e&v=9.4.1&x2=0)](https://www.npmjs.com/package/cypress/v/9.4.1) 


Install Cypress for Mac, Linux, or Windows, then [get started](https://docs.cypress.io/guides/getting-started/installing-cypress.html).

```bash
cd ../dgb-e2e-automation/ 
```

```bash
npm install
```


## Running Tests

To run the tests, follow the steps below


```bash
cd /your/project/path
```

and

```bash
npm run open
```

## Environment Variables

During the execution of this project, you will be able to define in which environment you want the tests to be executed. 
Just change the run command like this:

Staging environment:

```bash
cypress open -e configFile=staging’
```
Production environment:

```bash
cypress open -e configFile=production’
```

The environment settings can be consulted in the directory:

../config/


