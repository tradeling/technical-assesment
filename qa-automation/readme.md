# Coding task for QA Automation Engineer @tradeling

## The Goal

Your task is to write some end-to-end tests with [Cypress](https://www.cypress.io) to demonstrate your test automation abilities.

## What you'll need

1. The [Cypress Docs](https://docs.cypress.io)
1. The platform: [binance trading platform](https://www.binance.com/en)

## The Process

1. Start a new private github repository.
1. Initiate new Cypress project environment
1. Write some end-to-end tests fulfilling the [Acceptance Criteria](#acceptance-criteria) below
1. Push your code in Github. And give the access to following users: [Meabed](https://github.com/meabed)

## Acceptance Criteria

1. Write a first end-to-end test that
   1. Starts on the [Tradeling home page](https://tradeling.com/)
   1. On the nav bar click the category link Food & Beverage
   1. Click on Meat & Poultry
   1. Capture the total number of results from breadcrumbs
   1. Verify that the total results equals the sum of product count on each page

1. Write a second end-to-end test that
   1. Starts on the [Tradeling home page](https://tradeling.com/)
   1. On the nav bar click on the category link Office & Stationery
   1. Click on Office Supplies & Stationery
   1. Select Writing Instrument on filter by product type
   1. Select Ballpoint Pens on filter by product
   1. Apply filter by price between 50 and 60
   1. Verify that the total results are correct as per the filter applied

1. Write a third end-to-end test that
   1. Starts on the [Tradeling home page](https://mytrade.link/en)
   1. Verify that following category with sub category images are displaying on home screen
        - Health and Wellbeing
        - Food  & Beverages
        - Office Supplies


 **Publish test report in html format using custom code or cypress reporter plugin.**
## Bonus Round (not required, but nice-to-have)

- Usage of code quality tools such as eslint, prettier, typescript
- Integration of your tests into a CI pipeline
- Manual test cases for given scenarios
- Brief Performance report on home page using Jmeter or any similar tool
- Security and Vulnerability assessment
- Surprise us…

## How we're evaluating the result

Prioritized from most important to least important, here are our evaluation criteria:

1. **Acceptance Criteria**: Have all acceptance criteria been fulfilled correctly?
1. **Code Quality**: Is the code that you've written clean, well-structured and easy to understand?
1. **Documentation**: Did you document how to run your tests well? Is your written communication clear and easy-to-understand?
1. **The extra mile**: Everything you did on top of the acceptance criteria. See [Bonus Round](#bonus-round)
