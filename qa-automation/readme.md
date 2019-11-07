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
   1. Starts on the [landing page](https://www.binance.com/en)
   1. Click the link [view more market](https://www.binance.com/en/markets)
   1. Clicks the ETH/BTC button leading to [Pair trading view](https://www.binance.com/en/trade/ETH_BTC)
   1. Verifies that all important information is loaded, e.g. trading chart, limit, market, stop limit input boxes, etc. (leaving this purposefully open to see what you think makes sense to test)
   
1. Write a second end-to-end test that
   1. Starts on the [Pair trading view](https://www.binance.com/en/trade/ETH_BTC)
   1. Enters some valid values into the Buy ETH form
   1. Make sure the Total field has the correct value (Total = price \* Amount)
   1. Verifies that you can't submit the form since you are not logged in
   
1. Write a data last end-to-end (WebSockets) test that
   1. Starts on the [Pair trading view](https://www.binance.com/en/trade/ETH_BTC)
   1. Under the hood, the UI uses WebSockets to fetch tickers
   1. Verifies that the data is loaded in the tickers,
   1. Verifies there is a consistent stream of data.
   1. Verifies the time it takes the socket connection to connect is less than 1 second

## Bonus Round (not required, but nice-to-have)

- Usage of code quality tools such as eslint, prettier, typescript
- Integration of your tests into a CI pipeline
- Screenshot diffing
- Surprise us…

## How we're evaluating the result

Prioritized from most important to least important, here are our evaluation criteria:

1. **Acceptance Criteria**: Have all acceptance criteria been fulfilled correctly?
1. **Code Quality**: Is the code that you've written clean, well-structured and easy to understand?
1. **Documentation**: Did you document how to run your tests well? Is your written communication clear and easy-to-understand?
1. **The extra mile**: Everything you did on top of the acceptance criteria. See [Bonus Round](#bonus-round)
