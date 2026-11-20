# Shopping Cart Test Cases

> **Demo application:** [SauceDemo](https://www.saucedemo.com) (public practice site by Sauce Labs). These are sample test cases written for portfolio purposes.

**Module:** Shopping Cart  
**Total test cases:** 10

| TC ID | Title | Type | Priority |
|---|---|---|---|
| [TC_023](#tc_023) | Add a single product to cart | Functional / Smoke | High |
| [TC_024](#tc_024) | Add multiple products to cart | Functional | High |
| [TC_025](#tc_025) | Remove product from Products page | Functional | High |
| [TC_026](#tc_026) | Remove product from Cart page | Functional | High |
| [TC_027](#tc_027) | Cart page shows correct product details | Functional | High |
| [TC_028](#tc_028) | Continue Shopping from cart | Functional | Medium |
| [TC_029](#tc_029) | Cart is retained after page refresh | Functional | Medium |
| [TC_030](#tc_030) | Add to cart from product detail page | Functional | Medium |
| [TC_031](#tc_031) | Cart is retained after logout and login | Functional | Low |
| [TC_032](#tc_032) | Cart badge is hidden when cart is empty | UI | Low |

---

### TC_023

**Title:** Add a single product to cart  
**Type:** Functional / Smoke  
**Priority:** High  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Click "Add to cart" on Sauce Labs Backpack

**Expected Result:** Button changes to "Remove" and cart badge shows 1

---

### TC_024

**Title:** Add multiple products to cart  
**Type:** Functional  
**Priority:** High  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Click "Add to cart" on three products

**Expected Result:** Cart badge shows 3

---

### TC_025

**Title:** Remove product from Products page  
**Type:** Functional  
**Priority:** High  
**Precondition:** One product is already in cart  
**Test Data:** -

**Steps:**

1. Click "Remove" on that product

**Expected Result:** Button changes back to "Add to cart" and badge is removed

---

### TC_026

**Title:** Remove product from Cart page  
**Type:** Functional  
**Priority:** High  
**Precondition:** Two products are in cart  
**Test Data:** -

**Steps:**

1. Open cart
2. Click "Remove" on one product

**Expected Result:** Product is removed from the list and badge shows 1

---

### TC_027

**Title:** Cart page shows correct product details  
**Type:** Functional  
**Priority:** High  
**Precondition:** Product is added to cart  
**Test Data:** -

**Steps:**

1. Click the cart icon

**Expected Result:** Cart shows QTY 1, correct name, description and price

---

### TC_028

**Title:** Continue Shopping from cart  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Cart page  
**Test Data:** -

**Steps:**

1. Click "Continue Shopping"

**Expected Result:** User returns to Products page and cart items are retained

---

### TC_029

**Title:** Cart is retained after page refresh  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** Two products are in cart  
**Test Data:** -

**Steps:**

1. Refresh the browser page

**Expected Result:** Cart badge still shows 2 and products remain in cart

---

### TC_030

**Title:** Add to cart from product detail page  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on a product detail page  
**Test Data:** -

**Steps:**

1. Click "Add to cart"

**Expected Result:** Badge count increases by 1 and button changes to "Remove"

---

### TC_031

**Title:** Cart is retained after logout and login  
**Type:** Functional  
**Priority:** Low  
**Precondition:** One product is in cart  
**Test Data:** standard_user

**Steps:**

1. Logout
2. Login again with the same user

**Expected Result:** Cart content is retained (as per current application behaviour)

---

### TC_032

**Title:** Cart badge is hidden when cart is empty  
**Type:** UI  
**Priority:** Low  
**Precondition:** Cart is empty  
**Test Data:** -

**Steps:**

1. Observe the cart icon

**Expected Result:** No badge number is displayed on the cart icon

---
