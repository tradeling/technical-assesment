# Coding task for Mobile QA Automation Engineer @tradeling

## The Goal

Your task is to write automated tests preferably with [Appium](https://appium.io/), or [Detox](https://github.com/wix/Detox/)  to demonstrate your test automation abilities.


## The Process

1. Start a new github repository with detailed "README" document on how to execute the tests.
1. Download Amazon Shopping Android or App Store Package (APK or IPA)
1. Write end-to-end tests fulfilling the [Acceptance Criteria](#acceptance-criteria) below.
1. Publish test execution report in html format.
1. Prepare a test summary report and include the information about platform, app, tools etc
1. Include all tests related document in same github repository.

- Use below package and activity name (Appium)
  - appPackage=com.amazon.mShop.android.shopping
  - appActivity=com.amazon.mShop.home.HomeActivity

## Acceptance Criteria

- Scenario 1: [Check Add a new Payment to your profile]
   1. Open Amazon app with region United State
   2. Login with valid credentials
   3. Tap on Your account
   4. From Payments section, select Your Payments
   5. Tap on Wallet and add a credit or debit card as the payment method
   6. Assert on added card with correct type [Visa/Mastercard]


- Scenario 2: [Check your gift card's balance is $0.00]
   1. Tap on Your account
   2. From Payments section, select Manage gift card balance
   3. Check the balance of your gift card is $0.00


- Scenario 3: [Check the total displayed number of results for category Smart Home | Televisions]
   1. Click on Shop by Department from burger menu
   2. Choose category ‘Electronics’
   3. Choose sub-category category ’TV & VIDEO’
   4. Filter with ’Smart TV’ and click show results
   5. Check the total number of results match the total displayed in filter

- Scenario 4: [Check Add a new Address to your profile]
    1. Tap on Your account
    2. From Account settings, select Your Address
    3. Add new address
    4. Assert on added address under personal Addresses

- Scenario 5: [Check the selected currency displayed for the products' price]
    1. Go to Currency Settings
    2. Select Country & Language
    3. Change currency from 'USD' to 'AED'
    4. Save changes
    5. Assert on selected currency displayed for Deals and Promotions products

- Scenario 6: [Check Product Detail Page image swipe, Payments Option, Pricing, Stock, Add to Cart ]
    1. Tap on the Search bar and search for "Apple"
    2. Tap the picture of the product and swipe Left to Right
    3. The price of the product is displayed
    4. Verify payment options are displayed
    5. Verify out of stock or in stock, information is showing on the page.
    6. Tap and verify add to cart feature

## Bonus Round (not required, but nice-to-have)

- Integration of your tests into a CI pipeline
- Manual test cases to cover the given scenarios
- BDD integration with any BDD framework (Cucumber, Serenity etc)
- Surprise us…

## How we're evaluating the results

Prioritized from most important to least important, here are our evaluation criteria:

1. **Acceptance Criteria**: Have all acceptance criteria been fulfilled correctly?
1. **Code Quality**: Is the code that you've written clean, well-structured and easy to understand?
1. **Documentation**: Did you document how to run your tests well? Is your written communication clear and easy-to-understand?
1. **The extra mile**: Everything you did on top of the acceptance criteria.

## How to submit your work

Create a public repo on Github and push your code on it. then share the link back with the team.
