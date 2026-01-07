





Test Cases- Sauce Demo

---

##TC_001 - Login with valid credentials
**Precondition:** User is on login page
**Steps:**
1. Enter valid username:
'standard_user'
2. Enter valid password:
'secret_sauce'
3. Click Login button

**Expected Result:** User is redirected to Products page
**Status:** Pass

---

##TC_002 - Login with invalid password
**Steps:**
1. Enter valid username:
'standard_user'
2. Enter invalid password
3. Click Login button

**Expected Result:** Error message "Username and password do not match any user in this service"
User stays on login page
**Status:** Pass

---

##TC_003 - Login with locked out user
**Steps:**
1. Enter locked username:
'locked_out_user'
2. Enter valid password:
'secret_sauce'
3. Click Login button

**Expected Result:** Error message "Sorry, this user has been locked out"
**Status:** Pass

---

##TC_004 - Add product to cart
**Precondition:** User is logged in 
**Steps:**
1. Navigate to Products page
2. Click "Add to cart" on any product

**Expected Result:** Products added to cart, cart count increases
**Status** Pass

---

##TC_005 - Checkout process
**Precondition:** At least one product in cart
**Steps:**
1. Go to Card
2. Click "Checkout"
3. Fill First Name, Last Name, Zip/Postal code
4. Click "Continue"
5. Click "Finish"

**Expected Result:** Order completed page displayed with confirmation message
**Status:** Pass
