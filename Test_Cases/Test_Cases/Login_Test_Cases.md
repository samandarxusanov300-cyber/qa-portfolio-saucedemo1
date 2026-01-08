# Login Test Cases - Sauce Demo

---
## TC_001 - Login with valid credentials

**Precondition:** 
User is on login page

**Steps:**
1. Enter valid username:
'standard_user'
2. Enter valid password:
'secret_sauce'
3. Click the Login button

**Expected Result:**
User is redirected to the Products page

**Status:** Pass

---
## TC_002 - Login with invalid username

**Precondition:** 
User is on the login page

**Steps:**
1. Enter invalid username:
'invalid_user'
2. Enter valid password:
'secret_sauce'
3. Click the Login button

**Expected Result:**
Error message displayed:
"Username and password do not match any user in this service"

**Status:** Pass

---
## TC_003 - Login with invalid password

**Precondition:**
User is on the login page

**Steps:**
1. Enter valid username:
'standard_user'
2. Enter invalid password:
'invalid_password'
3. Click the Login button

**Expected Result:**
Error message displayed:
"Username and password do not match any user in this service"

**Status:** Pass

---
## TC_004 - Login with empty fields

**Precondition:**
User is on the login page

**Steps:**
1. Leave the username field empty
2. Leave the password field empty
3. Click the Login button

**Expected Result:**
Error message displayed:
"Epic sadface: Password is required"

**Status:** Pass

---
## TC_005 - Login with locked out user

**Precondition:**
User is on the login page

**Steps:**
1. Enter locked out username:
'locked_out_user'
2. Enter valid password:
'secret_sauce'
3. Click the Login button

**Expected Result:**
Error message displayed:
"Epic sadface: Sorry, this user has been locked out."

**Status:** Pass
