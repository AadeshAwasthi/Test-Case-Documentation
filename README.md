# Test Case Documentation

![Test Cases](https://img.shields.io/badge/Test%20Cases-60-blue) ![Type](https://img.shields.io/badge/Testing-Manual-green) ![Status](https://img.shields.io/badge/Project-Demo-orange)

Sample manual test cases written by **Aadesh Awasthi** (QA Engineer) to show how I design and document test cases.

> **Note:** This is a **demo project**. All test cases are written for [SauceDemo](https://www.saucedemo.com), a public practice website by Sauce Labs. No company or client data is used here.

## Application Under Test

| Item | Details |
|---|---|
| Application | SauceDemo (Swag Labs) |
| URL | https://www.saucedemo.com |
| Type | E-commerce web application (demo) |
| Test users | `standard_user`, `locked_out_user`, `problem_user` (shown on the login page) |

## Test Case Summary

| Module | Test Cases |
|---|---|
| [Login](test-cases/01_Login.md) | 12 |
| [Product Listing](test-cases/02_Product_Listing.md) | 10 |
| [Shopping Cart](test-cases/03_Cart.md) | 10 |
| [Checkout](test-cases/04_Checkout.md) | 12 |
| [Navigation Menu and Footer](test-cases/05_Navigation_Menu.md) | 8 |
| [UI and Browser Compatibility](test-cases/06_UI_Compatibility.md) | 8 |
| **Total** | **60** |

## Folder Structure

```
Test-Case-Documentation
├── README.md
├── test-cases
│   ├── 01_Login.md
│   ├── 02_Product_Listing.md
│   ├── 03_Cart.md
│   ├── 04_Checkout.md
│   ├── 05_Navigation_Menu.md
│   ├── 06_UI_Compatibility.md
│   └── All_Test_Cases.csv      (all cases in one sheet, opens in Excel)
└── templates
    └── Test_Case_Template.md
```

## Test Design Techniques Used

- Equivalence Partitioning (valid and invalid login data)
- Boundary and empty-field checks (checkout form)
- Positive and negative testing
- Error guessing (direct URL access, browser Back after logout)
- UI, responsive and browser compatibility checks

## Related Repositories

- [Manual-Testing-Portfolio](https://github.com/AadeshAwasthi/Manual-Testing-Portfolio) – test plan, strategy, checklists and execution reports
- [Bug-Report-Examples](https://github.com/AadeshAwasthi/Bug-Report-Examples) – sample bug reports
- [Selenium-Java-Automation](https://github.com/AadeshAwasthi/Selenium-Java-Automation) – automation examples for the same application
