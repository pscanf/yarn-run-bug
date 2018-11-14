# yarn-run-bug

Likely due to [yarnpkg/yarn #6650](https://github.com/yarnpkg/yarn/issues/6650).

## System info

-   node v10.13.0
-   yarn v1.12.3

## Reproduce

-   clone this repo and install dependencies
-   run `npm run coverage` and notice how the report says coverage is **100%**
-   run `yarn run coverage` and notice how the report says coverage is **0%**

![Reproduction video](./repro.gif)

## Npm scripts

-   `test` runs tests with mocha
-   `coverage` runs `nyc yarn test`, to calculate code coverage
