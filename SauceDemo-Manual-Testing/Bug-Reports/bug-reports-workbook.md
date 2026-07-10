# Bug Reports — SauceDemo Manual Testing

Defects found during test execution and exploratory testing.
All bugs reproduced twice before reporting.

**Tester:** [Your Name]
**Date:** [Date you tested]
**Environment:** [Your browser + version], [Your OS], https://www.saucedemo.com

---

## BUG-001 — All product images show the same incorrect image for problem_user

**Environment:** [Chrome 126 / Windows 11 — put YOUR actual browser and OS]
**Account:** problem_user / secret_sauce
**Related test case:** [Your TC ID for product image verification]

**Steps to reproduce:**
1. Go to https://www.saucedemo.com
2. Log in as problem_user / secret_sauce
3. Observe the product listing page

**Expected result:** Each of the 6 products displays its own correct image (backpack, bike light, t-shirt, etc.)

**Actual result:** All 6 products display an identical dog image.

**Severity:** High | **Priority:** High

**Reasoning:** Product images directly drive purchase decisions in e-commerce. Wrong images on 100% of the catalog would cause wrong orders, returns, and lost revenue on a real store.

**Screenshot:** screenshots/bug-001-product-images.png

---

## BUG-002 — [Write a title: sorting dropdown has no effect for problem_user]

> HOW TO FIND IT: Log in as problem_user. Note the current product order.
> Select "Name (Z to A)" from the sort dropdown, then "Price (low to high)".
> Watch what happens to the order. Delete these hint lines after writing.

**Environment:** [Your browser / OS]
**Account:** problem_user / secret_sauce
**Related test case:** [Your TC ID]

**Steps to reproduce:**
1. [Write the exact steps you performed]
2.
3.

**Expected result:** [What should a sort dropdown do?]

**Actual result:** [Describe exactly what you observed — was any error shown?]

**Severity:** Medium | **Priority:** Medium

**Reasoning:** [Why Medium/Medium? Think: core browsing feature fails silently, but a workaround exists with only 6 products. Write this in your own words.]

**Screenshot:** screenshots/bug-002-sort.png

---

## BUG-003 — [Write a title: checkout accepts empty Last Name for error_user]

> HOW TO FIND IT: Log in as error_user, add any item to cart, go to
> checkout. Fill First Name and Postal Code but leave Last Name EMPTY.
> Click Continue. Compare with what happens when First Name is empty.

**Environment:** [Your browser / OS]
**Account:** error_user / secret_sauce
**Related test case:** [Your TC ID — this should be one of your negative test cases]

**Steps to reproduce:**
1.
2.
3.
4.

**Expected result:** [What error message appears for the OTHER empty fields? The same should happen here.]

**Actual result:** [What actually happened?]

**Severity:** Medium | **Priority:** High

**Reasoning:** [Why is priority HIGHER than severity here? Hint: incomplete shipping data breaks order fulfillment downstream, and validation is inconsistent across fields of the same form.]

**Screenshot:** screenshots/bug-003-lastname.png

---

## BUG-004 — [Write a title: Finish button does not complete order for error_user]

> HOW TO FIND IT: As error_user, add an item, complete checkout up to
> the Overview page, then click Finish. Try clicking multiple times.
> BONUS for your report: press F12, open the Console tab, click Finish
> again, and note any red error — mentioning it makes your report stand out.

**Environment:** [Your browser / OS]
**Account:** error_user / secret_sauce
**Related test case:** [Your TC ID]

**Steps to reproduce:**
1.
2.
3.

**Expected result:** [What should Finish do?]

**Actual result:** [What happened? Include the console error if you found one.]

**Severity:** High | **Priority:** High

**Reasoning:** [Why is this the most serious bug in your report? Think about what it blocks.]

**Screenshot:** screenshots/bug-004-finish.png

---

## BUG-005 — [Write a title for a visual bug you find as visual_user]

> HOW TO FIND IT: Log in as visual_user and browse the site. Compare
> against standard_user in another browser window. Look at button
> positions, prices, and images. Pick ONE clear visual difference.

**Environment:** [Your browser / OS]
**Account:** visual_user / secret_sauce
**Related test case:** [TC ID, or write "Exploratory session"]

**Steps to reproduce:**
1.
2.

**Expected result:** [Consistent layout/styling with standard_user's view]

**Actual result:** [Describe the specific visual problem you chose]

**Severity:** Low | **Priority:** Low

**Reasoning:** [Why Low/Low? One sentence — cosmetic, functionality unaffected.]

**Screenshot:** screenshots/bug-005-visual.png

---

## Summary

| Bug ID | Title | Severity | Priority | Status |
|--------|-------|----------|----------|--------|
| BUG-001 | [title] | High | High | Open |
| BUG-002 | [title] | Medium | Medium | Open |
| BUG-003 | [title] | Medium | High | Open |
| BUG-004 | [title] | High | High | Open |
| BUG-005 | [title] | Low | Low | Open |
