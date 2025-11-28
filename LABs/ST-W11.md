
# ST W11. TestScript 


**Task:**
You are required to design and execute a full functional test for the **Fahasa online bookstore** ([https://www.fahasa.com](https://www.fahasa.com)).

### **Requirements:**

1. **Create a Test Script**

   * Write a complete test script (test steps, expected results, and test data).
   * The script must follow a clear structure: *Test Case ID, Test Objective, Preconditions, Steps, Expected Results.*

2. **Test Scenario – Online Book Purchase Flow**
   You will test the functional flow of searching and purchasing books on the Fahasa website.

   Specifically:

   * Identify **three specific books** you intend to purchase.
   * Use the website’s search function to search for each of the three books, one by one.
   * For every book found:

     * Open the book’s detail page.
     * Verify that the book information is displayed correctly.
     * Add the book to the shopping cart.

3. **Cart Verification**

   * After adding all three books to the cart, open the shopping cart page.
   * Verify the following:

     * All three selected books appear in the cart.
     * Quantity of each item is correct (default quantity = 1).
     * Prices (individual and total) are displayed.

4. **Checkout Process**

   * Proceed to the checkout page.
   * Verify that the checkout page loads correctly and displays required fields such as:

     * Customer information
     * Delivery address
     * Payment options
   * You are **not required** to complete an actual payment. Stopping before the payment confirmation is acceptable.

5. **Deliverables**

   * Test script (in table or structured text format).
   * Screenshots of test execution steps (optional but recommended).
   * A short summary of all issues/defects found, if any.

### **Notes**

* Students may use manual testing or automation tools (e.g., Selenium, Playwright, Cypress) depending on instructor guidance.
* Ensure all test cases are reproducible and written clearly.

---

Nếu bạn muốn, mình có thể **tạo luôn bộ test cases mẫu**, hoặc **viết bản automation bằng Selenium/Python/Playwright**.
