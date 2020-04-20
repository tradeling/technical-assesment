# Coding task for QA Automation Engineer @tradeling

## The Goal

Your task is to write automated tests preferably with [Cypress](https://www.cypress.io), [NightWatch](https://nightwatchjs.org/) or [Puppeteer](https://pptr.dev/) to demonstrate your test automation abilities.



## The Process

1. Start a new private github repository.
1. Write end-to-end tests fulfilling the [Acceptance Criteria](#acceptance-criteria) below
1. Prepare a test summary report and include the information about platform, browser, tools etc

## Acceptance Criteria

1. Write a first end-to-end test that
   1. Starts on the [Binance market page](https://www.binance.com/en/markets)
   1. On the search box (coin name) type ETH
   1. Check if last price updates in every 5 second
   1. Clear the last price on search box
   1. Mark ETH , BNB as favorites
   1. Verify if Pair's are displayed under Favorites link

1. Write a second end-to-end test that
   1. Select ETH on "ALTS Markets" filter
   1. Verify that pair column is sorted with all ETH values
   1. Select USSD on "FIAT Markets" filter
   1. Verify that  pair column is sorted with all USSD values
   1. And ALTS Markets filter default value is reset to "All"

1. Write a third end-to-end test that
   1. Verify on the top navigation bar "Spot" list has following values :
        Basic, Classic, Advance, OTC, P2P
   2. Make sure the "ETH/USDT" ticker price changes constantly



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
