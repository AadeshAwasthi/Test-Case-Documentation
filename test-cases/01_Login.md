# Login Test Cases

> **Demo application:** [SauceDemo](https://www.saucedemo.com) (public practice site by Sauce Labs). These are sample test cases written for portfolio purposes.

**Module:** Login  
**Total test cases:** 12

| TC ID | Title | Type | Priority |
|---|---|---|---|
| [TC_001](#tc_001) | Login with valid standard user | Functional / Smoke | High |
| [TC_002](#tc_002) | Login with invalid password | Negative | High |
| [TC_003](#tc_003) | Login with invalid username | Negative | High |
| [TC_004](#tc_004) | Login with empty username and password | Negative | Medium |
| [TC_005](#tc_005) | Login with empty password | Negative | Medium |
| [TC_006](#tc_006) | Login with locked out user | Negative | High |
| [TC_007](#tc_007) | Password field masks the characters | UI | Medium |
| [TC_008](#tc_008) | Error message can be dismissed | UI | Low |
| [TC_009](#tc_009) | Login using Enter key | Functional | Low |
| [TC_010](#tc_010) | Username is case sensitive | Negative | Medium |
| [TC_011](#tc_011) | Direct URL access without login | Security | High |
| [TC_012](#tc_012) | Leading and trailing spaces in username | Negative | Low |

---

### TC_001

**Title:** Login with valid standard user  
**Type:** Functional / Smoke  
**Priority:** High  
**Precondition:** User is on the login page  
**Test Data:** standard_user / secret_sauce

**Steps:**

1. Enter username
2. Enter password
3. Click Login

**Expected Result:** User is redirected to /inventory.html and the Products page is displayed

---

### TC_002

**Title:** Login with invalid password  
**Type:** Negative  
**Priority:** High  
**Precondition:** User is on the login page  
**Test Data:** standard_user / wrong_pass

**Steps:**

1. Enter valid username
2. Enter wrong password
3. Click Login

**Expected Result:** Error "Username and password do not match any user in this service" is displayed; user stays on login page

---

### TC_003

**Title:** Login with invalid username  
**Type:** Negative  
**Priority:** High  
**Precondition:** User is on the login page  
**Test Data:** invalid_user / secret_sauce

**Steps:**

1. Enter unregistered username
2. Enter valid password
3. Click Login

**Expected Result:** Same mismatch error message is displayed

---

### TC_004

**Title:** Login with empty username and password  
**Type:** Negative  
**Priority:** Medium  
**Precondition:** User is on the login page  
**Test Data:** -

**Steps:**

1. Leave both fields blank
2. Click Login

**Expected Result:** Error "Epic sadface: Username is required" is displayed

---

### TC_005

**Title:** Login with empty password  
**Type:** Negative  
**Priority:** Medium  
**Precondition:** User is on the login page  
**Test Data:** standard_user

**Steps:**

1. Enter username
2. Leave password blank
3. Click Login

**Expected Result:** Error "Epic sadface: Password is required" is displayed

---

### TC_006

**Title:** Login with locked out user  
**Type:** Negative  
**Priority:** High  
**Precondition:** User is on the login page  
**Test Data:** locked_out_user / secret_sauce

**Steps:**

1. Enter locked user credentials
2. Click Login

**Expected Result:** Error "Sorry, this user has been locked out." is displayed

---

### TC_007

**Title:** Password field masks the characters  
**Type:** UI  
**Priority:** Medium  
**Precondition:** User is on the login page  
**Test Data:** secret_sauce

**Steps:**

1. Type any text in the Password field

**Expected Result:** Characters are shown as dots; field type is password

---

### TC_008

**Title:** Error message can be dismissed  
**Type:** UI  
**Priority:** Low  
**Precondition:** An error message is displayed on login page  
**Test Data:** -

**Steps:**

1. Click the X icon on the error banner

**Expected Result:** Error banner disappears and red field icons are removed

---

### TC_009

**Title:** Login using Enter key  
**Type:** Functional  
**Priority:** Low  
**Precondition:** User is on the login page  
**Test Data:** standard_user / secret_sauce

**Steps:**

1. Enter valid username and password
2. Press Enter key

**Expected Result:** User is logged in without clicking the Login button

---

### TC_010

**Title:** Username is case sensitive  
**Type:** Negative  
**Priority:** Medium  
**Precondition:** User is on the login page  
**Test Data:** STANDARD_USER / secret_sauce

**Steps:**

1. Enter username in upper case
2. Enter valid password
3. Click Login

**Expected Result:** Login fails with the mismatch error message

---

### TC_011

**Title:** Direct URL access without login  
**Type:** Security  
**Priority:** High  
**Precondition:** User is logged out  
**Test Data:** -

**Steps:**

1. Open /inventory.html directly in a new browser session

**Expected Result:** User is redirected to login page with error "You can only access '/inventory.html' when you are logged in."

---

### TC_012

**Title:** Leading and trailing spaces in username  
**Type:** Negative  
**Priority:** Low  
**Precondition:** User is on the login page  
**Test Data:** " standard_user "

**Steps:**

1. Enter username with a space before and after
2. Enter valid password
3. Click Login

**Expected Result:** Spaces are not trimmed. Login fails with the error "Username and password do not match any user in this service"

---
