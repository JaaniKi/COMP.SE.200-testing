# Student template

## Purpose of this repository

This is a project template for students participating in Software Testing course
at Tampere University.

The repository only contains the source code that is under testing, `package.json` skeleton
and LICENSE file.

Source code folder contains a separate license file that must **NOT** be removed under any circumstances!
Removing this license file directly violates terms and conditions of the software under testing.
Individuals who remove or modify the license file will also carry the consequences.


# COMP.SE.200 Testing

Coveralls badge:
[![Coverage Status](https://coveralls.io/repos/github/JaaniKi/COMP.SE.200-testing/badge.svg?branch=main)](https://coveralls.io/github/JaaniKi/COMP.SE.200-testing?branch=main)

Unit tests for a utility library that is evaluated for use in an e-commerce store (COMP.SE.200 Software Testing, Tampere University).

The `src/.internal` directory is assumed to work and is excluded from tests and coverage reports. Do not remove the license file inside `src/`.

## Running the tests locally

Requirements: Git and Node.js (v22 is used in CI).

```bash
npm ci               # install dependencies
npm test             # run the unit tests (Mocha + Chai)
npm run coverage     # run the tests and generate the coverage report (c8)
```

The coverage report is printed to the console and written to `coverage/lcov.info`.

## Continuous integration

Every push and pull request runs the GitHub Actions workflow (`.github/workflows/ci.yml`). It installs Node.js and the dependencies, runs the tests with coverage, and sends the lcov report to Coveralls.

## Test suite naming

- `[Plan]`: test cases designed in the test plan (part 1)
- `[AI-generated]`: test cases created with AI assistance
- `[valid]`, `[invalid]`, `[edge]`: other tests, grouped by input type

## Testing status

| Source file | Planned test cases | Implemented | Passing | Related issues |
|---|---|---|---|---|
| add.js | | | | |
| ceil.js | | | | |
| toNumber.js | | | | |
| reduce.js | | | | |
| defaultTo.js | | | | |
| toString.js | | | | |
| filter.js | | | | |
| chunk.js | | | | |
| isEmpty.js | | | | |
| upperFirst.js | | | | |

A failing test means a defect was found. Failing tests are not removed. Each one is documented in a GitHub issue that is linked in the table.