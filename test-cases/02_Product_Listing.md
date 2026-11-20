# Product Listing Test Cases

> **Demo application:** [SauceDemo](https://www.saucedemo.com) (public practice site by Sauce Labs). These are sample test cases written for portfolio purposes.

**Module:** Product Listing  
**Total test cases:** 10

| TC ID | Title | Type | Priority |
|---|---|---|---|
| [TC_013](#tc_013) | All six products are displayed | Functional / Smoke | High |
| [TC_014](#tc_014) | Sort products by Name (A to Z) | Functional | Medium |
| [TC_015](#tc_015) | Sort products by Name (Z to A) | Functional | Medium |
| [TC_016](#tc_016) | Sort products by Price (low to high) | Functional | Medium |
| [TC_017](#tc_017) | Sort products by Price (high to low) | Functional | Medium |
| [TC_018](#tc_018) | Open product details by clicking product name | Functional | High |
| [TC_019](#tc_019) | Open product details by clicking product image | Functional | Medium |
| [TC_020](#tc_020) | Back to products from detail page | Functional | Medium |
| [TC_021](#tc_021) | Each product shows its own correct image | UI | Medium |
| [TC_022](#tc_022) | Price format is correct | UI | Low |

---

### TC_013

**Title:** All six products are displayed  
**Type:** Functional / Smoke  
**Priority:** High  
**Precondition:** User is logged in  
**Test Data:** -

**Steps:**

1. Observe the Products page

**Expected Result:** 6 products are listed, each with name, description, price, image and Add to cart button

---

### TC_014

**Title:** Sort products by Name (A to Z)  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Select "Name (A to Z)" from sort dropdown

**Expected Result:** Products are listed in ascending alphabetical order

---

### TC_015

**Title:** Sort products by Name (Z to A)  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Select "Name (Z to A)" from sort dropdown

**Expected Result:** Products are listed in descending alphabetical order

---

### TC_016

**Title:** Sort products by Price (low to high)  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Select "Price (low to high)"

**Expected Result:** First product is $7.99 and last product is $49.99

---

### TC_017

**Title:** Sort products by Price (high to low)  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Select "Price (high to low)"

**Expected Result:** First product is $49.99 and last product is $7.99

---

### TC_018

**Title:** Open product details by clicking product name  
**Type:** Functional  
**Priority:** High  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Click on "Sauce Labs Backpack" title

**Expected Result:** Product detail page opens with the same name, description and price

---

### TC_019

**Title:** Open product details by clicking product image  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Click on the image of any product

**Expected Result:** Detail page of the same product opens

---

### TC_020

**Title:** Back to products from detail page  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on a product detail page  
**Test Data:** -

**Steps:**

1. Click "Back to products"

**Expected Result:** User returns to the Products page

---

### TC_021

**Title:** Each product shows its own correct image  
**Type:** UI  
**Priority:** Medium  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Compare each product image with its name

**Expected Result:** Every product has a unique, relevant image; no broken images

---

### TC_022

**Title:** Price format is correct  
**Type:** UI  
**Priority:** Low  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Check price of every product

**Expected Result:** Every price is shown as $ followed by a value with two decimals

---
