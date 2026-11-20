# Checkout Test Cases

> **Demo application:** [SauceDemo](https://www.saucedemo.com) (public practice site by Sauce Labs). These are sample test cases written for portfolio purposes.

**Module:** Checkout  
**Total test cases:** 12

| TC ID | Title | Type | Priority |
|---|---|---|---|
| [TC_033](#tc_033) | Checkout with valid information | Functional / Smoke | High |
| [TC_034](#tc_034) | Checkout with empty First Name | Negative | High |
| [TC_035](#tc_035) | Checkout with empty Last Name | Negative | High |
| [TC_036](#tc_036) | Checkout with empty Postal Code | Negative | High |
| [TC_037](#tc_037) | Cancel on information page | Functional | Medium |
| [TC_038](#tc_038) | Item total is calculated correctly | Functional | High |
| [TC_039](#tc_039) | Tax and Total are calculated correctly | Functional | High |
| [TC_040](#tc_040) | Finish the order | Functional / Smoke | High |
| [TC_041](#tc_041) | Back Home after order completion | Functional | Medium |
| [TC_042](#tc_042) | Cancel on overview page | Functional | Medium |
| [TC_043](#tc_043) | Payment and shipping information are displayed | UI | Low |
| [TC_044](#tc_044) | Checkout with empty cart | Negative | Medium |

---

### TC_033

**Title:** Checkout with valid information  
**Type:** Functional / Smoke  
**Priority:** High  
**Precondition:** At least one product is in cart  
**Test Data:** Aadesh / Awasthi / 452001

**Steps:**

1. Open cart and click Checkout
2. Enter First Name, Last Name, Postal Code
3. Click Continue

**Expected Result:** Checkout: Overview page is displayed

---

### TC_034

**Title:** Checkout with empty First Name  
**Type:** Negative  
**Priority:** High  
**Precondition:** User is on Checkout: Your Information  
**Test Data:** - / Awasthi / 452001

**Steps:**

1. Leave First Name blank
2. Fill other fields
3. Click Continue

**Expected Result:** Error "Error: First Name is required" is displayed

---

### TC_035

**Title:** Checkout with empty Last Name  
**Type:** Negative  
**Priority:** High  
**Precondition:** User is on Checkout: Your Information  
**Test Data:** Aadesh / - / 452001

**Steps:**

1. Leave Last Name blank
2. Fill other fields
3. Click Continue

**Expected Result:** Error "Error: Last Name is required" is displayed

---

### TC_036

**Title:** Checkout with empty Postal Code  
**Type:** Negative  
**Priority:** High  
**Precondition:** User is on Checkout: Your Information  
**Test Data:** Aadesh / Awasthi / -

**Steps:**

1. Leave Postal Code blank
2. Fill other fields
3. Click Continue

**Expected Result:** Error "Error: Postal Code is required" is displayed

---

### TC_037

**Title:** Cancel on information page  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Checkout: Your Information  
**Test Data:** -

**Steps:**

1. Click Cancel

**Expected Result:** User returns to the Cart page; items are retained

---

### TC_038

**Title:** Item total is calculated correctly  
**Type:** Functional  
**Priority:** High  
**Precondition:** Two products are in cart and user is on Overview page  
**Test Data:** Backpack $29.99 + Bike Light $9.99

**Steps:**

1. Add the prices of all listed items
2. Compare with "Item total"

**Expected Result:** Item total shows $39.98

---

### TC_039

**Title:** Tax and Total are calculated correctly  
**Type:** Functional  
**Priority:** High  
**Precondition:** User is on Overview page  
**Test Data:** Item total $39.98

**Steps:**

1. Check Tax value
2. Verify Total = Item total + Tax

**Expected Result:** Tax is $3.20 and Total is $43.18

---

### TC_040

**Title:** Finish the order  
**Type:** Functional / Smoke  
**Priority:** High  
**Precondition:** User is on Overview page  
**Test Data:** -

**Steps:**

1. Click Finish

**Expected Result:** "Thank you for your order!" message is displayed on the "Checkout: Complete!" page

---

### TC_041

**Title:** Back Home after order completion  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** Order is completed  
**Test Data:** -

**Steps:**

1. Click "Back Home"

**Expected Result:** User is on Products page and the cart is empty

---

### TC_042

**Title:** Cancel on overview page  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is on Overview page  
**Test Data:** -

**Steps:**

1. Click Cancel

**Expected Result:** User returns to Products page; order is not placed

---

### TC_043

**Title:** Payment and shipping information are displayed  
**Type:** UI  
**Priority:** Low  
**Precondition:** User is on Overview page  
**Test Data:** -

**Steps:**

1. Observe Payment Information and Shipping Information

**Expected Result:** Payment card reference and shipping method text are displayed

---

### TC_044

**Title:** Checkout with empty cart  
**Type:** Negative  
**Priority:** Medium  
**Precondition:** Cart is empty  
**Test Data:** -

**Steps:**

1. Open cart
2. Click Checkout

**Expected Result:** User should not be allowed to proceed to checkout with an empty cart

---
