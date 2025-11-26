# Regression Checklist – ShopX E-Commerce

This is a small regression checklist to re-run after major changes or bug fixes.

| Area     | Check Item                                      | Status       | Notes                 |
|----------|--------------------------------------------------|-------------|-----------------------|
| Login    | User can log in with valid credentials          | Not Run     |                       |
| Login    | Invalid credentials show correct error message  | Not Run     |                       |
| Search   | Search returns results for valid product names  | Not Run     |                       |
| Cart     | Adding an item updates cart count and total     | Not Run     |                       |
| Cart     | Removing an item updates cart total             | Not Run     | Related to BUG-002    |
| Checkout | Checkout flow completes for a simple order      | Not Run     | No real payment used  |
| Orders   | New order appears in order history              | Not Run     |                       |
