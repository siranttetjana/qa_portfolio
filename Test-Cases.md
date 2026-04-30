# Test Cases

This document contains test cases for e-commerce cart functionality, including positive and negative test scenarios.

---

### TC001: Verify that user can add product to cart

**Preconditions:**
- User is on product page

**Steps:**
1. Open product page
2. Click "Add to Cart" button

**Expected Result:**
- Product is added to the cart
- Cart icon shows updated quantity
- Product details are displayed correctly in cart

---

### TC002: Verify that user can update product quantity in cart

**Preconditions:**
- Product is added to the cart

**Steps:**
1. Open cart page
2. Increase product quantity
3. Click "Update" (if applicable)

**Expected Result:**
- Quantity is updated
- Total price is recalculated accordingly

---

### TC003: Verify that user can remove product from cart

**Preconditions:**
- Product is added to the cart

**Steps:**
1. Open cart page
2. Click "Remove" button

**Expected Result:**
- Product is removed from the cart
- Cart is updated correctly

---

### TC004: Verify cart persistence after browser restart

**Preconditions:**
- Product is added to the cart

**Steps:**
1. Add product to cart
2. Close browser
3. Reopen browser
4. Navigate to website

**Expected Result:**
- Cart retains previously added items

---

### TC005: Verify cart behavior after page refresh

**Preconditions:**
- Product is added to the cart

**Steps:**
1. Add product to cart
2. Refresh the page

**Expected Result:**
- Cart content remains unchanged

---

### TC006: Verify that user cannot set negative quantity

**Preconditions:**
- Product is added to the cart

**Steps:**
1. Open cart page
2. Enter "-1" in quantity field
3. Click "Update"

**Expected Result:**
- System prevents invalid input
- Validation message is displayed

---

### TC007: Verify maximum allowed quantity per product

**Preconditions:**
- Product is added to the cart

**Steps:**
1. Open cart page
2. Enter a large number (e.g., 9999)
3. Click "Update"

**Expected Result:**
- Quantity is limited to maximum allowed value
- Appropriate message is shown

---

### TC008: Verify cart icon updates after adding product

**Preconditions:**
- User is on product page

**Steps:**
1. Click "Add to Cart"

**Expected Result:**
- Cart icon displays correct number of items

---

### TC009: Verify cart is empty after removing all products

**Preconditions:**
- Multiple products added to cart

**Steps:**
1. Open cart page
2. Remove all products

**Expected Result:**
- Cart is empty
- "Cart is empty" message is displayed
