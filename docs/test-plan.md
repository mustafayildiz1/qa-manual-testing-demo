# Test Plan – ShopX E-Commerce

## 1. Scope

This test plan covers basic functional testing for a simple e-commerce web application called **ShopX**.

Included in scope:
- User registration & login
- Product listing & search
- Cart operations (add / remove items)
- Checkout (without real payment integration)
- Order history (view past orders)

Out of scope for this demo:
- Performance testing
- Security testing
- Cross-browser and mobile device matrix
- Real payment gateway integration

---

## 2. Test Types

- **Smoke Testing**  
  Basic check that the main flows (login, add to cart, checkout) work.

- **Functional Testing**  
  Verifying that each feature behaves as expected based on requirements.

- **Regression Testing (limited)**  
  Re-running key test cases after a bug fix or change.

---

## 3. Test Environment

- Browser: Google Chrome (latest stable version)  
- OS: Windows 10  
- Test environment URL:  
  `https://test.shopx-demo.local` (fictional address for this project)

---

## 4. Entry & Exit Criteria

**Entry Criteria:**
- Test environment is accessible
- A stable build is deployed
- Basic smoke tests pass (site loads, login page available)

**Exit Criteria:**
- No open **Critical** or **High** severity bugs
- Major flows (login, search, cart, checkout) pass functional tests
- Known minor issues are documented

---

## 5. Risks & Assumptions

- Payment processing is simulated, not connected to real banks
- No heavy load/users are simulated (no performance testing)
- Requirements are simple and may not reflect a real production app
