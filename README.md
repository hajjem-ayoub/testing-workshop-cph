# testing-workshop-cph [![CircleCI][ci-badge]][ci-url]

> End-to-end testing workshop with [Cypress.io](https://www.cypress.io/) at CopenhagenJS / ngCopenhagen

## Requirements

- Any computer: Mac, Windows, Linux
- [Node 6+](https://nodejs.org/)
- [git](https://git-scm.com)

In order to get the code and install dependencies

```shell
git clone git@github.com:cypress-io/testing-workshop-cph.git
cd testing-workshop-cph
npm install
```

## Application

[Vue.js](https://vuejs.org/) + [Vuex](https://vuex.vuejs.org/) + REST server application that we are going to test is in the folder `todomvc`. This application and its full testing is described in [this blog post](https://www.cypress.io/blog/2017/11/28/testing-vue-web-application-with-vuex-data-store-and-rest-backend/).

## Slides

[https://gitpitch.com/cypress-io/testing-workshop-cph][presentation] with the starting file in [PITCHME.md](PITCHME.md) presented using [GitPitch](https://gitpitch.com/). The pitch file includes files from the [slides](slides) folder. Students should open the [presentation slides][presentation] and follow along.

[presentation]: https://gitpitch.com/cypress-io/testing-workshop-cph

## Content

Strike through for topics we are going to skip.

| topics                                 | folder                                                                                   | slides                                                        |
| -------------------------------------- | ---------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| Introduction, TodoMVC application      | [todomvc](todomvc)                                                                       | [intro.md](slides/intro.md)                                   |
| `cypress open` vs `cypress run`        | [cypress/integration/01-basic](cypress/integration/01-basic)                             | [01-basic.md](slides/01-basic.md)                             |
| Adding items test, `cypress.json` file | [cypress/integration/02-adding-items](cypress/integration/02-adding-items)               | [02-adding-items.md](slides/02-adding-items.md)               |
| ~~Selector Playground~~                    | [cypress/integration/03-selector-playground](cypress/integration/03-selector-playground) | [03-selector-playground.md](slides/03-selector-playground.md) |
| Reset database using `cy.request`      | [cypress/integration/04-reset-state](cypress/integration/04-reset-state)                 | [04-reset-state.md](slides/04-reset-state.md)                 |
| Spy and stub XHR requests, fixtures    | [cypress/integration/05-xhr](cypress/integration/05-xhr)                                 | [05-xhr.md](slides/05-xhr.md)                                 |
| Access application code and data       | [cypress/integration/06-app-data-store](cypress/integration/06-app-data-store)           | [06-app-data-store.md](slides/06-app-data-store.md)           |
| Setting up E2E tests on CI             | [cypress/integration/07-ci](cypress/integration/07-ci)                                   | [07-ci.md](slides/07-ci.md)                                   |
| ~~Setting up Cypress Dashboard~~           | [cypress/integration/07-ci](cypress/integration/07-ci)                                   | [08-dashboard.md](slides/08-dashboard.md)                     |
| The end                                | -                                                                                        | [end.md](slides/end.md)                                       |

## For speakers

During the workshop, keep the `todomvc` app running in one shell, while each section `01-basic`, `02-...`, `03-...` etc. has its own Cypress and specs subfolders `cypress/integration/...`. Usually a spec has several tests with placeholder comments. The workshop attendees are expected to make the tests pass using the knowledge from the slides and hints (and [Cypress documentation](https://docs.cypress.io/)). Note that most folders have a prepared `spec.js` file and an `answer.js` file. The `answer.js` file is ignored by Cypress using a setting in `cypress.json`.

The slides can be shown directly via the [presentation link][presentation] above. The Markdown files in [slides](slides) folder also has a little bit of speaker notes.

[ci-badge]: https://circleci.com/gh/cypress-io/testing-workshop-cph.svg?style=svg
[ci-url]: https://circleci.com/gh/cypress-io/testing-workshop-cph
