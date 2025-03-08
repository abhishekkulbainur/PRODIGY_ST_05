# Automated Checkout Process Script

## Purpose
This script automates the checkout process on an e-commerce website using **Selenium WebDriver** and **Python**. The process includes adding an item to the cart, filling out the checkout forms, and verifying the success message upon purchase.

## Steps
1. Open the e-commerce website.
2. Navigate to a product page and add an item to the cart.
3. Proceed to the checkout process, filling in the login and address forms.
4. Choose the payment method and confirm the order.
5. Verify that the success message is displayed upon successful order completion.

## Script Output

1. **Page Transitions**: 
   - Successful navigation between the cart, login, checkout, and payment pages.
   - No issues with page transitions.

2. **Form Validations**:
   - **Login Form**: Successfully filled out and submitted.
   - **Address Form**: Address, city, postcode, and phone number successfully entered.
   - **Payment Form**: 'Pay by bank wire' option selected and the order confirmed.

3. **Success Message Verification**:
   - The message "Your order on My Store is complete." was successfully verified.

## Issues Encountered

- **Issue**: Occasionally, the product page takes longer to load than expected, causing the script to timeout. 
   - **Solution**: Implementing **explicit waits** for elements to load resolves the issue.
- **Issue**: Payment confirmation page sometimes fails to load.
   - **Solution**: Re-attempt the page load with a longer timeout and check the element visibility.

## Recommendations for Improvement
- Enhance the robustness of the script by adding error handling for network issues.
- Add more advanced verification like checking for email confirmation after the order.
