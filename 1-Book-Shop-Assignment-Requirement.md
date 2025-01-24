## Project Overview & Objective:

Create a Book Shop application with user-friendly features, secure authentication, and smooth product management. Ensure the platform is responsive, error-free, and visually appealing.

* * *

## Main Functionalities: 45 Marks

### 1\. **User Registration & Authentication (Role-Based)**

*   **Secure Registration and Login:**
    *   Users can register with the following fields: `name`, `email, and` `password.` **_By default the registered user will have the_** **_user_** **_role._**
    **Note:** You will have to update a user to admin manually. No need to implement the super admin functionality.
    *   Passwords must be securely hashed before storing in the database.
    *   Users can log in using their `email` and `password`.
*   **JWT (JSON Web Token):**
    *   Generate a JWT token upon login for secure authentication.
    *   Store the token in local storage to maintain user sessions.
*   **Logout:**
    *   Clear the token from local storage upon logout and **redirect the user to the login page**.

* * *

### 2\. **Public Routes**

1. **Home Page:**
    *   **Navbar**: Include a logo, favicon, navigation items, and buttons for login/signup and other interactions where necessary.
    *   **Banner**: Highlight your platform or special offers. You can use carousel if you want.
    *   **Featured Products**: Display up to 6 products with a "View All" button. On clicking the **View All** button, the user will be redirected to the All Products Page.
    *   **Extra Section**: Add relevant e-commerce content, such as testimonials or blogs.
    *   **Footer**: Include essential links, social media icons, and contact details.
2. **All Products Page:**
        *   **Search Functionality:** Allow users to search by title, author, or category.
        *   **Filters:** Include options for `price range`, `author`, `category`, and `availability`.
        *   **Dynamic Results:** Results should be updated based on search terms or selected filters.
        *   **Product Cards:** Show details like name, author, price, and category.
        *   Include a "View Details" button for each product.
3. **Product Details Page:**
    *   Display the product image and detailed information.
    *   Provide a "Buy Now" button that redirects to the checkout page.
4. **About Page:**
    *   Create an informative page about your shop and its mission.
    *   Add any other relevant details.

* * *

### 3\. **Private Routes**

1. **Checkout Page:**
    *   Users can place orders for products.
    *   Ensure the ordered quantity does not exceed the product stock.
        *   **Order Form:** Include product details, user details, total price calculation, and payment method.
        *   **Payment Integration:** Integrate SurjoPay as the payment gateway.
    *   Include an "Order Now" button to confirm the purchase.
2. **Dashboard (Role-Based Access):**
        *   **Admin Dashboard:** Features include managing users (e.g., deactivating accounts), managing products (CRUD), and managing orders(CRUD).
        *   **User Dashboard:** Features include viewing orders and managing profile settings.
        *   Allow users to update passwords (require current password for security).

* * *

## **UI/UX Design: 15 Marks**

*   **Responsive Design:**
    *   Ensure the platform works seamlessly on all screen sizes.
    *   Use proper alignment, typography, and intuitive layouts.
*   **Error Handling:**
    *   Show user-friendly error messages for:
        *   Invalid login credentials.
        *   Registration errors (e.g., duplicate email).
        *   Failed operations (e.g., out-of-stock products).
*   **Loading States:**
    *   Display spinners or loaders during API calls, such as on login or data fetch.
*   **Toasts:**
    *   Notify users of important actions (e.g., "Login successful", "Order placed", etc).

* * *

## Recommendation Functionalities (Optional)

**Product Review Section:**

*   Allow users to add reviews for specific products from the **Product Details Page**.
*   Include fields like `rating` (e.g., 1–5 stars) and `comment` for the review.
*   Other users can view all reviews for a product on the same page.
*   Ensure user reviews are displayed with the reviewer’s name, rating, and comment.
