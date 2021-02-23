# Coding task for Web QA Automation Engineer @tradeling

## The Goal

Your task is to write automated tests preferably with [Cypress](https://www.cypress.io), [NightWatch](https://nightwatchjs.org/) or [Playwright](https://playwright.dev/) to demonstrate your test automation abilities.


## The Process

1. Start a new github repository with detailed "README" document on how to execute the tests.
1. Write end-to-end tests fulfilling the [Acceptance Criteria](#acceptance-criteria) below.
1. Publish test execution report in html format.
1. Prepare a test summary report and include the information about platform, browser, tools etc
1. Include all tests related document in same github repository.


## Acceptance Criteria

- Scenario 1: [Check your gift card's balance is $0.00]
   1. Starts on the [Amazon](https://www.amazon.com/)
   2. Login with valid credentials
   3. Click on Your account
   4. Click on Gift Cards
   5. Check the balance of your gift card is $0.00


- Scenario 2: [Check the total displayed number of results for category Smart Home | Televisions]
   1. Go to Categories list
   2. Choose category 'Smart Home'
   3. Choose sub-category category 'Home Entertainment'
   4. Choose sub-category 'Televisions'
   5. Check the total number of results match the total displayed products


- Scenario 3: [Check the selected currency displayed for the products' price]
   1. Go to Currency Settings
   2. Change currency from 'USD' to 'AED'
   3. Save changes
   4. Check the selected currency displayed for the products' price


## Bonus Round (not required, but nice-to-have)

- Usage of code quality tools such as eslint, prettier, typescript
- Integration of your tests into a CI pipeline
- Manual test cases to cover the given scenarios
- Brief Performance report on home page using Jmeter or any similar tool
- Security and Vulnerability assessment
- Surprise us…

## How we're evaluating the results

Prioritized from most important to least important, here are our evaluation criteria:

1. **Acceptance Criteria**: Have all acceptance criteria been fulfilled correctly?
1. **Code Quality**: Is the code that you've written clean, well-structured and easy to understand?
1. **Documentation**: Did you document how to run your tests well? Is your written communication clear and easy-to-understand?
1. **The extra mile**: Everything you did on top of the acceptance criteria.

## How to submit your work

Create a public repo on Github and push your code on it. then share the link back with the team.
