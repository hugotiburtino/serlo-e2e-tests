# Serlo E2E Tests

That is a suggestion of integration tests for serlo.org.
It uses Cucumber for BDD and Selenium for Browser testing.

## Getting started

You need node, yarn, docker and chromium (or chrome) installed.

1. `yarn` to install dependencies
2. Run the Serlo's [frontend](https://github.com/serlo/frontend/blob/staging/README.md#getting-started).
   _Important_: make sure to set in `.env.local` `NEXT_PUBLIC_ENV=local` as this repo does not support running tests against the staging environment, yet.
3. Run in `frontend` in branch `kratos`: `yarn kratos:detach`, `yarn kratos: prepare`
4. Come back to this repo: `yarn up` to run the docker containers for api, db layer etc.
5. `yarn test`

## Running tests

- `yarn test` - to run all tests
- `yarn test <file>` - to run tests of an specific file

## TODOs

- [ ] Make it easily configurable to different environments
- [ ] Setup CI-CD pipeline to run tests against staging
- [ ] Change easily the repo to be tested
- [ ] Less imperative, more declarative tests, making it possible though to be easily configurable
