# UI and Browser Compatibility Test Cases

> **Demo application:** [SauceDemo](https://www.saucedemo.com) (public practice site by Sauce Labs). These are sample test cases written for portfolio purposes.

**Module:** UI and Browser Compatibility  
**Total test cases:** 8

| TC ID | Title | Type | Priority |
|---|---|---|---|
| [TC_053](#tc_053) | Login page on Google Chrome | Compatibility | Medium |
| [TC_054](#tc_054) | Login page on Mozilla Firefox | Compatibility | Medium |
| [TC_055](#tc_055) | Login page on Microsoft Edge | Compatibility | Medium |
| [TC_056](#tc_056) | Products page on mobile viewport | Responsive | Medium |
| [TC_057](#tc_057) | Products page on tablet viewport | Responsive | Low |
| [TC_058](#tc_058) | Page zoom at 150% | UI | Low |
| [TC_059](#tc_059) | Keyboard Tab order on login page | Usability | Low |
| [TC_060](#tc_060) | Header elements alignment | UI | Low |

---

### TC_053

**Title:** Login page on Google Chrome  
**Type:** Compatibility  
**Priority:** Medium  
**Precondition:** Latest Chrome is installed  
**Test Data:** standard_user

**Steps:**

1. Open the application URL
2. Login with valid user

**Expected Result:** Page renders correctly and login works

---

### TC_054

**Title:** Login page on Mozilla Firefox  
**Type:** Compatibility  
**Priority:** Medium  
**Precondition:** Latest Firefox is installed  
**Test Data:** standard_user

**Steps:**

1. Open the application URL
2. Login with valid user

**Expected Result:** Page renders correctly and login works

---

### TC_055

**Title:** Login page on Microsoft Edge  
**Type:** Compatibility  
**Priority:** Medium  
**Precondition:** Latest Edge is installed  
**Test Data:** standard_user

**Steps:**

1. Open the application URL
2. Login with valid user

**Expected Result:** Page renders correctly and login works

---

### TC_056

**Title:** Products page on mobile viewport  
**Type:** Responsive  
**Priority:** Medium  
**Precondition:** Browser DevTools is available  
**Test Data:** -

**Steps:**

1. Set viewport to 375 x 667
2. Open Products page

**Expected Result:** Products are shown in a single column; no horizontal scroll bar

---

### TC_057

**Title:** Products page on tablet viewport  
**Type:** Responsive  
**Priority:** Low  
**Precondition:** Browser DevTools is available  
**Test Data:** -

**Steps:**

1. Set viewport to 768 x 1024
2. Open Products page

**Expected Result:** Layout adjusts properly; no overlapping elements

---

### TC_058

**Title:** Page zoom at 150%  
**Type:** UI  
**Priority:** Low  
**Precondition:** User is on Products page  
**Test Data:** -

**Steps:**

1. Set browser zoom to 150%

**Expected Result:** Text and buttons remain readable and clickable

---

### TC_059

**Title:** Keyboard Tab order on login page  
**Type:** Usability  
**Priority:** Low  
**Precondition:** User is on the login page  
**Test Data:** -

**Steps:**

1. Press Tab repeatedly from the top of the page

**Expected Result:** Focus moves Username > Password > Login in order

---

### TC_060

**Title:** Header elements alignment  
**Type:** UI  
**Priority:** Low  
**Precondition:** User is logged in  
**Test Data:** -

**Steps:**

1. Observe logo, menu icon and cart icon

**Expected Result:** All header elements are aligned and not overlapping

---
