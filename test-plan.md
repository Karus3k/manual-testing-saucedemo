# Test plan

## What I test
SauceDemo web shop: https://www.saucedemo.com

Areas:
1. Login
2. Product list (sorting, product page)
3. Cart (add, remove)
4. Checkout (form, summary, finish)
5. Menu and logout

Not in scope: performance, security, API.

## Test users
All users have the password shown on the login page.

| User | Why I use it |
|---|---|
| standard_user | normal flow, should work |
| locked_out_user | login should be blocked |
| problem_user | known bugs in the UI |
| error_user | known bugs in actions |
| visual_user | visual differences |
| performance_glitch_user | slow login |

## Environment
- Windows, Chrome (latest)
- Desktop window, later also mobile view in DevTools

## How
- Write test cases first, then run them and fill the result (Pass / Fail).
- Every Fail gets a bug report in `bug-reports/`.
- Some exploratory testing at the end of each area, notes added to the bug reports or test cases.
