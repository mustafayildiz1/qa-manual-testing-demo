# Test Cases – ShopX E-Commerce

Below is a simple list of example test cases for core flows.

---

## Login

| ID            | Module | Title                      | Preconditions          | Steps                                                                 | Expected Result                                  |
|---------------|--------|----------------------------|------------------------|-----------------------------------------------------------------------|-------------------------------------------------|
| TC-LOGIN-001  | Login  | Valid login                | User account exists    | 1. Go to login page  2. Enter valid email and password  3. Click Login | User is redirected to the dashboard/home page. |
| TC-LOGIN-002  | Login  | Invalid password           | User account exists    | 1. Go to login page  2. Enter valid email + wrong password  3. Click Login | Error message is shown. User stays on login page. |
| TC-LOGIN-003  | Login  | Empty fields validation    | None                   | 1. Go to login page  2. Leave fields empty  3. Click Login              | Validation messages are displayed for required fields. |

---

## Product Search

| ID              | Module | Title                       | Preconditions                | Steps                                                                 | Expected Result                                              |
|-----------------|--------|-----------------------------|------------------------------|-----------------------------------------------------------------------|-------------------------------------------------------------|
| TC-SEARCH-001   | Search | Search existing product     | Product "Keyboard" exists    | 1. Go to home page  2. Enter "Keyboard" in search bar  3. Click Search | List shows at least one product with "Keyboard" in the name. |
| TC-SEARCH-002   | Search | Search non-existing product | None                         | 1. Go to home page  2. Enter random string "xyz123"  3. Click Search   | No results message is shown.                               |

---

## Cart & Checkout

| ID                | Module | Title                          | Preconditions               | Steps                                                                                                 | Expected Result                                                  |
|-------------------|--------|--------------------------------|-----------------------------|-------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| TC-CART-001       | Cart   | Add single product to cart    | Product listing is visible  | 1. Go to product listing  2. Click "Add to cart" on a product                                         | Cart icon/summary shows 1 item.                               |
| TC-CART-002       | Cart   | Remove product from cart      | Cart has at least 1 product | 1. Go to cart page  2. Click "Remove" on an item                                                      | Item is removed and cart total is updated.                    |
| TC-CHECKOUT-001   | Checkout | Successful checkout (no payment) | User logged in & cart filled | 1. Go to cart  2. Click "Proceed to checkout"  3. Confirm order on summary page                       | Order confirmation page is displayed, order appears in history. |
