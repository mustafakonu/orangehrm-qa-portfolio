# Login Test Cases

## TC_LOGIN_001

**Title:** Successful login with valid credentials

**Preconditions:** User account exists

**Test Data:**

* Username: Admin
* Password: admin123

**Steps:**

1. Open login page
2. Enter valid username
3. Enter valid password
4. Click Login

**Expected Result:**
User is redirected to Dashboard.

**Priority:** High

**Type:** Functional

---

## TC_LOGIN_002

**Title:** Login with invalid password

**Preconditions:** User account exists

**Test Data:**

* Username: Admin
* Password: WrongPassword

**Steps:**

1. Open login page
2. Enter valid username
3. Enter invalid password
4. Click Login

**Expected Result:**
Error message is displayed.

**Priority:** High

**Type:** Negative

---

## TC_LOGIN_003

**Title:** Login with invalid username

**Test Data:**

* Username: WrongUser
* Password: admin123

**Steps:**

1. Open login page
2. Enter invalid username
3. Enter valid password
4. Click Login

**Expected Result:**
Error message is displayed.

**Priority:** High

**Type:** Negative

---

## TC_LOGIN_004

**Title:** Login with empty username

**Steps:**

1. Open login page
2. Leave username empty
3. Enter password
4. Click Login

**Expected Result:**
Required field validation message appears.

**Priority:** High

**Type:** Validation

---

## TC_LOGIN_005

**Title:** Login with empty password

**Steps:**

1. Open login page
2. Enter username
3. Leave password empty
4. Click Login

**Expected Result:**
Required field validation message appears.

**Priority:** High

**Type:** Validation

---

## TC_LOGIN_006

**Title:** Login with both fields empty

**Steps:**

1. Open login page
2. Leave username empty
3. Leave password empty
4. Click Login

**Expected Result:**
Validation messages appear for both fields.

**Priority:** High

**Type:** Validation

---

## TC_LOGIN_007

**Title:** Password field masks entered characters

**Steps:**

1. Open login page
2. Enter password

**Expected Result:**
Password characters are hidden.

**Priority:** Medium

**Type:** UI

---

## TC_LOGIN_008

**Title:** Login using leading spaces in username

**Steps:**

1. Open login page
2. Enter username with leading spaces
3. Enter valid password
4. Click Login

**Expected Result:**
System trims spaces or displays proper validation.

**Priority:** Medium

**Type:** Boundary

---

## TC_LOGIN_009

**Title:** Login using SQL injection text

**Test Data:**

* Username: ' OR '1'='1

**Steps:**

1. Open login page
2. Enter SQL injection string
3. Enter any password
4. Click Login

**Expected Result:**
Login should fail.

**Priority:** High

**Type:** Security

---

## TC_LOGIN_010

**Title:** Logout after successful login

**Preconditions:** User logged in

**Steps:**

1. Click profile menu
2. Click Logout

**Expected Result:**
User is redirected to Login page.

**Priority:** High

**Type:** Functional
