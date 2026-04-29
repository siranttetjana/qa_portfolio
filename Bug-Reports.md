# Bug Reports Portfolio

This document contains sample bug reports created during practice testing of demo web applications.  
The reports demonstrate my ability to identify UI, functional, and usability issues, determine severity/priority, and document defects clearly.

---

## BUG-001: Second product card height differs from other product cards

**Type:** UI Bug  
**Severity:** Minor  
**Priority:** Medium  
**Status:** Open  
**Environment:** Windows 10 Pro / Chrome 140.0.7339.128

### Steps to Reproduce
1. Open https://academybugs.com/find-bugs/  
2. Observe the second product card **"Dark Grey Jeans"**

### Expected Result
All product cards have the same height and aligned layout.

### Actual Result
The second product card has a smaller height than the other product cards.

### Impact
Inconsistent UI layout reduces visual quality of the page.

---

## BUG-002: Grand Total is calculated incorrectly in cart

**Type:** Functional Bug  
**Severity:** Critical  
**Priority:** High  
**Status:** Open  
**Environment:** Windows 10 Pro / Chrome 140.0.7339.128

### Steps to Reproduce
1. Open https://academybugs.com/find-bugs/  
2. Add any product to cart  
3. Click **Update** under the Quantity field  
4. Check the **Grand Total** amount

### Expected Result
Grand Total should equal **Cart Subtotal + Shipping**.

### Actual Result
Grand Total amount is displayed incorrectly.

### Impact
Incorrect final order amount may reduce user trust and affect purchases.

---

## BUG-003: Product price and currency do not change after selecting another currency

**Type:** Functional Bug  
**Severity:** Major  
**Priority:** Medium  
**Status:** Open  
**Environment:** Windows 10 Pro / Chrome 140.0.7339.128

### Steps to Reproduce
1. Open https://academybugs.com/find-bugs/  
2. Add any product to cart  
3. In **Select a Currency**, choose another currency

### Expected Result
Product prices and currency symbols should update according to selected currency.

### Actual Result
Prices and currency type remain unchanged.

### Impact
Users may see incorrect pricing information.

---

## BUG-004: Sign In button overlaps footer section

**Type:** UI Bug  
**Severity:** Minor  
**Priority:** Low  
**Status:** Open  
**Environment:** Windows 10 Pro / Chrome 140.0.7339.128

### Steps to Reproduce
1. Open https://academybugs.com/find-bugs/  
2. Add any product to cart  
3. Scroll to the bottom of the right-side menu

### Expected Result
Sign In button should be displayed correctly without overlapping other elements.

### Actual Result
Sign In button overlaps the footer section.

### Impact
Broken page layout creates poor user experience.

---

## BUG-005: Billing Address section does not load correctly

**Type:** Functional Bug  
**Severity:** Major  
**Priority:** Medium  
**Status:** Open  
**Environment:** Windows 10 Pro / Chrome 140.0.7339.128

### Steps to Reproduce
1. Open https://academybugs.com/find-bugs/  
2. Open any product page  
3. Log in or sign up  
4. Open **Dashboard**  
5. Navigate to **Billing Address** section

### Expected Result
Billing Address section should load and display user data correctly.

### Actual Result
Billing Address section behaves incorrectly / does not load as expected.

### Impact
Users may be unable to manage billing information.

---

## BUG-006: Product quantity cannot be increased above 2 in cart

**Type:** Functional Bug  
**Severity:** Major  
**Priority:** High  
**Status:** Open  
**Environment:** Windows 10 Pro / Chrome 140.0.7339.128

### Steps to Reproduce
1. Open https://academybugs.com/find-bugs/  
2. Add one or more products to cart  
3. Open **View Cart**  
4. Set quantity to 3 or more  
5. Click **Update**

### Expected Result
Product quantity should be increased according to available stock.

### Actual Result
Quantity cannot be increased above 2.

### Impact
Purchase quantity limitation may reduce sales and user satisfaction.