# Testing Angular 4 Apps with Jasmine
This repository contains the code of Testing Angular 4 Apps with Jasmine Course.

This course repository is updated to Angular v7, and there is a package-lock.json file available, for avoiding semantic versioning installation issues.

## Theory

**Unit test:** Tests components in isolation.
**Integration test:** Tests components with templates, API's, DB's, etc.
**End-to-end test:** Tests the flow right from the start to finish to check that it behaves as expected.

## Clean coding practices

* Create small functions (10 lines of code or less)
* Proper naming
* Single responsability

## Angular commands

* **ng test:** runs karma.
* **ng test --code-coverage:** creates a test code coverage report.

## Tests main parts

* **describe:** indicates a suite (set of tests).
* **it:** indicates a test (set of validations).
* **expect:** indicates a validation (set of validations).

## Test Structure (best practice)

* **Arrange:** initialize variables.
* **Act:** make actions (e.g.: call methods or functions).
* **Assert:** execute tests (e.g.: expects).

## Most used test methods

* **beforeEach:** used to initialize (set up) common variables for all tests.
* **afterEach:** used to clean up (tear down) common variables for all tests.
* **beforeAll:** executes once before all tests.
* **afterAll:** executes once after all tests.
* **toBe:** used mostly compare to numeric values (objects as well).
* **toContains:** checks it contains a specfied value. Used mostly to compare strings and arrays.
* **toBeTruthy:** checks if value is true.
* **toBeFalsy:** checks if value is false.
* **toBeNull:** checks if value is null.
* **toHaveBeenCalled:** checks if a method was called.
* **toHaveBeenCalledWith:** checks if a method was called with a value.
* **toGreaterThan:** checks if is greater than a value.

## spyOn method

Takes an object and inserts a spy in it (fakes it).
It is usually called with callFake or returnsValue methods:

* spyOn(object, 'methodName').and.callFake(fakeMethod)
* spyOn(object, 'methodName').and.returnsValue(value)

## Notes

* The ideal coverage is 70%.
* Adding an "x" before a "describe" or "it" method will make karma skip the suits or tests
