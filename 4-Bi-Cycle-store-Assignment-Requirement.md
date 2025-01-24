# #4 Bi-Cycle store Assignment

* * *

**Bicycle Store Application Requirements**

**Project Overview & Objective:** Develop a Bicycle Store application featuring user-friendly functionalities, secure authentication, and efficient product management. Ensure the application is responsive, free of errors, and visually appealing.

**Main Functionalities: 45 Marks**

1. **User Registration & Authentication (Role-Based)**
    *   **Secure Registration and Login:**
        *   Users can register by providing their name, email, and password. By default, users are assigned the "customer" role.
        *   Admin roles can be updated manually; no "super admin" feature is required.
        *   Passwords must be hashed securely before being stored in the database.
        *   Users log in using their email and password.
    *   **JWT (JSON Web Token):**
        *   Generate a JWT token upon login for secure authentication.
        *   Store the token in local storage to maintain user sessions.
    *   **Logout:**
        *   Remove the token from local storage upon logout and redirect users to the login page.
2. **Public Routes**
    *   **Home Page:**
        *   **Navbar:** Include a logo, navigation items, and buttons for login/signup and other actions.
        *   **Banner:** Showcase special offers or features using a carousel if preferred.
        *   **Featured Bicycles:** Display up to 6 bicycles with a "View All" button redirecting to the "All Bicycles" Page.
        *   **Extra Section:** Add content relevant to e-commerce, such as testimonials.
        *   **Footer:** Include important links, social media icons, and contact details.
    *   **All Bicycles Page:**
        *   **Search Functionality:** Allow users to search by brand, bicycle name, or category.
        *   **Filters:** Implement options for price range, model, brand, category, and availability.
        *   **Dynamic Results:** Update results based on search queries or selected filters.
        *   **Bicycle Cards:** Display details including name, brand, model, price, and category, with a "View Details" button for each.
    *   **Bicycle Details Page:**
        *   Show the bicycle image and detailed specifications.
        *   Provide a "Buy Now" button that redirects to the checkout page.
    *   **About Page:**
        *   Create a page detailing your bicycle shop and its mission, including any other relevant information.
3. **Private Routes**
    *   **Checkout Page:**
        *   Users can order bicycles.
        *   Ensure the ordered quantities do not exceed available stock.
        *   **Order Form:** Include product details, user details, total price calculation, and payment method.
        *   **Payment Integration:** Integrate SurjoPay or Stripe or any other payment gateway of your choice.
        *   Include an "Order Now" button to finalize the purchase.
    *   **Dashboard (Role-Based Access):**
        *   **Admin Dashboard:** Manage users (e.g., deactivate accounts), products (CRUD), and orders (CRUD).
        *   **User Dashboard:** View orders and manage profile settings. Allow users to update passwords (requiring the current password for security).

**UI/UX Design: 15 Marks**

*   **Responsive Design:**
    *   Ensure optimal performance across all screen sizes, maintaining alignment, typography, and intuitive layouts.
*   **Error Handling:**
    *   Provide user-friendly error messages for:
        *   Invalid login credentials.
        *   Registration issues (e.g., duplicate email).
        *   Failed operations (e.g., products out of stock).
*   **Loading States:**
    *   Display loaders or spinners during API calls like login or data fetching.
*   **Toasts:**
    *   Notify users of important actions (e.g., "Login successful," "Order placed," etc.).

**Recommendation Functionalities (Optional)**

*  **User Side:**
         **Bicycle Comparison Tool:**
               **User Side:**
                      *  Compare up to 3 bicycles side-by-side.
                      *   Display specifications, pricing, and features to help users make informed decisions.
  **Admin Side:**
  **Sales Dashboard:**
  **Overview Chart:**
        *   Display a summary of sales data with visual charts (e.g., bar charts, line charts, or pie charts) for better analysis.
  **Key Metrics:**
  **Total Sales Revenue**: Show total revenue over a selectable time period.
  **Units Sold**: Display the number of bicycles sold.
  **Top-Selling Bicycles**: Highlight the most popular models with sales figures.

## **Backend Requirements:**

*   **Database:** Use MongoDB with a schema including:
    *   Users (defined roles: customer, admin)
    *   Bicycles (with attributes like name, brand, price, model, stock)
    *   Orders (linked to user, product details, total price, status)
*   **Authentication:**
    *   Implement user registration, login, JWT token management, and logout.
    *   Ensure secure password hashing and user session handling.
*   **Product Management:**
    *   Implement CRUD operations for bicycles (create, read, update, delete).
*   **Order Management:**
    *   Execute CRUD operations for orders (create, read, update, delete), ensuring stock levels before orders are placed.
*   **Payment Integration:**
    *   Utilize SurjoPay/AmaarPay/SSLCommerz/Stripe for payment processing.
*   **Error Handling:**
    *   Establish consistent, user-friendly error messaging for invalid login attempts, out-of-stock bicycles, etc.
*   **Additional Changes:**
    *   Ensure backend APIs support pagination for bicycle listings and order retrieval.
    *   Add authentication middleware to protect private routes, including checkout and the dashboard

`You can use any existing backend if you have developed it earlier or create a new version modifying from the existing older one.`
