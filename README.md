🛒 E-commerce Playwright POM Framework (TypeScript)

A scalable End-to-End Test Automation Framework built using Playwright with TypeScript following the Page Object Model (POM) design pattern.

This project automates key user journeys of an E-commerce web application including browsing products, adding items to cart, managing wish lists, and completing checkout.

🚀 Tech Stack

Playwright – End-to-End testing framework

TypeScript – Strongly typed JavaScript

Page Object Model (POM) – Scalable automation design pattern

GitHub – Version control

Allure Report – Advanced reporting

Playwright HTML Reporter

📂 Project Structure
ecommerce-playwright-pom-framework-typescript
│
├── pages
│   ├── HomePage.ts
│   ├── CategoryPage.ts
│   ├── ProductPage.ts
│   ├── CheckoutPage.ts
│   └── LoginPage.ts
│
├── tests
│   ├── TC01_NavigateToLaptops.spec.ts
│   ├── TC02_SelectProduct.spec.ts
│   ├── TC03_AddToCart.spec.ts
│   ├── TC04_CompletePurchase.spec.ts
│   ├── TC05_AddToWishlist.spec.ts
│   └── TC06_AddAffiliate.spec.ts
├── utils
├── playwright-report
├── playwright.config.ts
├── package.json
├── tsconfig.json
│
└── README.md
🧩 Framework Design

This framework follows Page Object Model (POM) architecture.

Pages Layer

Contains:

UI Locators

Page actions

Reusable methods

Example:

ProductPage.ts
CheckoutPage.ts
LoginPage.ts
Test Layer

Contains:

Test scenarios

Assertions

Business workflows

🧪 Automated Test Scenarios

The framework includes 6 automated test cases covering major E-commerce workflows.

TC01 – Navigate to Laptops & Notebooks

Open application home page

Navigate to Laptops & Notebooks

Validate category page loads successfully

TC02 – Select Product

Navigate to category

Select product HP LP3065

Validate product details page

TC03 – Add Product to Cart

Select product

Set delivery date

Click Add to Cart

Validate success message

TC04 – Complete Purchase

Add product to cart

Navigate to checkout

Login during checkout

Select shipping address

Select shipping & payment method

Confirm order

Validate order success message

TC05 – Add Product to Wishlist

Open product page

Click Add to Wishlist

Validate success notification

TC06 – Add Affiliate

Navigate to affiliate section

Add affiliate details

Validate affiliate creation

▶️ Installation

Clone the repository:

git clone https://github.com/your-username/ecommerce-playwright-pom-framework-typescript.git

Go to project directory:

cd ecommerce-playwright-pom-framework-typescript

Install dependencies:

npm install

Install browsers:

npx playwright install
▶️ Running Tests

Run all tests:

npx playwright test

Run tests with visible browser:

npx playwright test --headed

Run in UI mode:

npx playwright test --ui

Run sanity tests:

npx playwright test --grep @sanity

Run regression tests:

npx playwright test --grep @regression
📊 Test Reports
Playwright HTML Report

Generate report:

npx playwright show-report

Report location:

playwright-report/index.html
Allure Report

Generate results:

npx playwright test

Generate report:

allure generate ./allure-results --clean

Open report:

allure open
✨ Framework Features

✔ Page Object Model architecture
✔ Reusable page methods
✔ Tag-based test execution
✔ Playwright HTML reporting
✔ Allure advanced reporting
✔ Clean TypeScript structure

🔮 Future Improvements

CI/CD integration using GitHub Actions

Parallel execution

Cross-browser testing

Test data management

API + UI automation integration

👩‍💻 Author

Josena Thomas
QA Automation Engineer
