# Test cases

Result: Pass / Fail / Not run. Every Fail has a link to a bug report.

## Login

| ID | Title | Steps | Expected result | Result |
|---|---|---|---|---|
| TC-01 | Login with correct data | 1. Open the login page 2. Enter `standard_user` and the correct password 3. Click Login | Product list page opens | Not run |
| TC-02 | Login with wrong password | 1. Enter `standard_user` and a wrong password 2. Click Login | Error message, user stays on login page | Not run |
| TC-03 | Login with empty fields | 1. Leave both fields empty 2. Click Login | Error: username is required | Not run |
| TC-04 | Login with empty password | 1. Enter `standard_user`, leave password empty 2. Click Login | Error: password is required | Not run |
| TC-05 | Locked out user | 1. Enter `locked_out_user` and the correct password 2. Click Login | Error that the user is locked out | Not run |
| TC-06 | Open product page without login | 1. Log out 2. Open https://www.saucedemo.com/inventory.html directly | User is sent back to login with an error | Not run |

## Products

| ID | Title | Steps | Expected result | Result |
|---|---|---|---|---|
| TC-07 | Sort by price low to high | 1. Log in 2. Choose "Price (low to high)" | Products sorted from cheapest | Not run |
| TC-08 | Sort by name Z to A | 1. Log in 2. Choose "Name (Z to A)" | Products sorted Z to A | Not run |
| TC-09 | Product page | 1. Log in 2. Click a product name | Product page with the same name, price and picture | Not run |

## Cart

| ID | Title | Steps | Expected result | Result |
|---|---|---|---|---|
| TC-10 | Add product to cart | 1. Log in 2. Click "Add to cart" on one product | Cart icon shows 1, button changes to "Remove" | Not run |
| TC-11 | Remove product from cart | 1. Add a product 2. Open cart 3. Click "Remove" | Product disappears, cart icon has no number | Not run |
| TC-12 | Cart keeps products after logout | 1. Add 2 products 2. Log out 3. Log in again | Check if the cart still has 2 products (write what happens) | Not run |

## Checkout

| ID | Title | Steps | Expected result | Result |
|---|---|---|---|---|
| TC-13 | Checkout with correct data | 1. Add a product 2. Cart > Checkout 3. Fill first name, last name, zip 4. Continue > Finish | "Thank you for your order" page | Not run |
| TC-14 | Checkout with empty first name | 1. Go to checkout 2. Leave first name empty 3. Continue | Error: first name is required | Not run |
| TC-15 | Checkout with empty cart | 1. Empty cart 2. Open cart 3. Click Checkout | Check if checkout is possible with an empty cart (write what happens) | Not run |
| TC-16 | Price summary | 1. Add 2 products 2. Go to checkout overview | Item total = sum of prices, Total = item total + tax | Not run |

## Menu

| ID | Title | Steps | Expected result | Result |
|---|---|---|---|---|
| TC-17 | Logout | 1. Log in 2. Menu > Logout | Login page opens | Not run |
| TC-18 | Reset app state | 1. Add a product 2. Menu > Reset App State | Cart is empty | Not run |
