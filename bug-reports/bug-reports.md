# Bug Reports – ShopX E-Commerce

Example bug reports written in a simple, JIRA-like format.

---

## BUG-001 – Login accepts invalid email format

**Module:** Login  
**Severity:** Medium  
**Priority:** High  
**Status:** Open

**Preconditions:**
- Test environment is available.

**Steps to Reproduce:**
1. Go to the login page.  
2. Enter `abc` as email (no "@" or domain).  
3. Enter any password.  
4. Click "Login".

**Expected Result:**
- Email field shows a validation error: "Please enter a valid email address."
- Login is not attempted.

**Actual Result:**
- No validation message is shown.
- Login request is sent and a generic "Invalid credentials" message appears.

---

## BUG-002 – Cart total not updated after removing item

**Module:** Cart  
**Severity:** High  
**Priority:** High  
**Status:** Open

**Preconditions:**
- User is logged in.
- Cart contains at least 2 items.

**Steps to Reproduce:**
1. Go to the cart page.  
2. Note the total price.  
3. Remove one of the items.  

**Expected Result:**
- The removed item disappears from the cart.
- Cart total is recalculated and decreased.

**Actual Result:**
- The item is removed visually.
- Cart total **does not change** and still includes the removed item.

---

## BUG-003 – Search results page shows broken image icons

**Module:** Search / Product Listing  
**Severity:** Low  
**Priority:** Medium  
**Status:** Open

**Preconditions:**
- At least one product in the database has a missing image URL.

**Steps to Reproduce:**
1. Search for a category that includes products with missing images.  
2. Open the search results page.

**Expected Result:**
- A default placeholder image is shown for products with missing images.

**Actual Result:**
- Broken image icons are displayed for some products.
