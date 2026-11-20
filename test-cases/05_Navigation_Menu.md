# Navigation Menu and Footer Test Cases

> **Demo application:** [SauceDemo](https://www.saucedemo.com) (public practice site by Sauce Labs). These are sample test cases written for portfolio purposes.

**Module:** Navigation Menu and Footer  
**Total test cases:** 8

| TC ID | Title | Type | Priority |
|---|---|---|---|
| [TC_045](#tc_045) | Open the side menu | Functional | Medium |
| [TC_046](#tc_046) | Logout from the application | Functional / Smoke | High |
| [TC_047](#tc_047) | Browser Back after logout | Security | High |
| [TC_048](#tc_048) | All Items link | Functional | Low |
| [TC_049](#tc_049) | About link | Functional | Low |
| [TC_050](#tc_050) | Reset App State | Functional | Medium |
| [TC_051](#tc_051) | Close the side menu | UI | Low |
| [TC_052](#tc_052) | Footer social links | Functional | Low |

---

### TC_045

**Title:** Open the side menu  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** User is logged in  
**Test Data:** -

**Steps:**

1. Click the burger menu icon

**Expected Result:** Menu opens with All Items, About, Logout and Reset App State

---

### TC_046

**Title:** Logout from the application  
**Type:** Functional / Smoke  
**Priority:** High  
**Precondition:** User is logged in  
**Test Data:** -

**Steps:**

1. Open menu
2. Click Logout

**Expected Result:** User is redirected to the login page

---

### TC_047

**Title:** Browser Back after logout  
**Type:** Security  
**Priority:** High  
**Precondition:** User has just logged out  
**Test Data:** -

**Steps:**

1. Click browser Back button

**Expected Result:** Protected page is not shown; user stays on / is sent to login page

---

### TC_048

**Title:** All Items link  
**Type:** Functional  
**Priority:** Low  
**Precondition:** User is on Cart page  
**Test Data:** -

**Steps:**

1. Open menu
2. Click All Items

**Expected Result:** Products page is displayed

---

### TC_049

**Title:** About link  
**Type:** Functional  
**Priority:** Low  
**Precondition:** User is logged in  
**Test Data:** -

**Steps:**

1. Open menu
2. Click About

**Expected Result:** Sauce Labs website (saucelabs.com) opens

---

### TC_050

**Title:** Reset App State  
**Type:** Functional  
**Priority:** Medium  
**Precondition:** Two products are in cart  
**Test Data:** -

**Steps:**

1. Open menu
2. Click Reset App State

**Expected Result:** Cart badge is cleared and all buttons show "Add to cart"

---

### TC_051

**Title:** Close the side menu  
**Type:** UI  
**Priority:** Low  
**Precondition:** Side menu is open  
**Test Data:** -

**Steps:**

1. Click the X icon

**Expected Result:** Menu closes and page is fully visible

---

### TC_052

**Title:** Footer social links  
**Type:** Functional  
**Priority:** Low  
**Precondition:** User is logged in  
**Test Data:** -

**Steps:**

1. Click Twitter, Facebook and LinkedIn icons in footer

**Expected Result:** Each link opens the correct Sauce Labs social page in a new tab

---
