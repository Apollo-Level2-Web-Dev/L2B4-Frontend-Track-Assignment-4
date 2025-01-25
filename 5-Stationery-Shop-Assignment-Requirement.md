### **Stationery Shop Assignment Requirements**

* * *

#### **Project Overview & Objective**

Create a stationery Shop application with user-friendly features, secure authentication, and smooth product management. Ensure the platform is responsive, error-free, and visually appealing.

* * *

### **Main Functionalities** (45 Marks)

#### 1\. **User Registration & Authentication (Role-Based)**

*   **Secure Registration and Login**:
    *   Users can register using the following fields: **name**, **email**, and **password**.
    *   By default, registered users will have the **user** role.
    *   There is no need to implement super admin functionality. Update the role to admin manually.
    *   Passwords must be securely hashed before storing in the database.
    *   Users can log in using their email and password.
    *   Avoid any kind of validations such as character limit, and need of special character.
*   **JWT (JSON Web Token)**:
    *   Generate a **JWT token** upon login for secure authentication.
    *   Store the token in **local storage** to maintain user sessions.
*   **Logout**:
    *   Clear the token from local storage upon logout.

* * *

#### 2\. **Public Routes**

*   **Home Page**:
    *   **Navbar**:
        *   Include a logo, navigation items, and buttons for login/signup.
    *   **Banner**:
        *   Highlight the platform or special offers using a hero section.
        *   **carousel** (optional).
    *   **Featured Products**:
        *   Display up to 6 products with a "View All" button.
        *   Clicking "View All" redirects the user to the **All Products Page**.
    *   **Relevant section**:
        *   Add e-commerce content like testimonials or blogs.
    *   **Footer**:
        *   Include essential links, social media icons, and contact details.
*   **All Products Page**:
    *   **Search Functionality**:
        *   Allow users to search by title, author, or category.
    *   **Filters**:
        *   Include options for **price range**, **category**, and **availability**.
    *   **Dynamic Results**:
        *   Update results based on search terms or selected filters.
    *   **Product Cards**:
        *   Display product details like **name**, **price**, and **category**.
        *   Include a **View Details** button for each product.
*   **Product Details Page**:
    *   Display the product image and detailed information.
    *   Provide an "Add to cart" button.
*   **About Page**:
    *   Create an informative page about your shop and its mission.

* * *

#### 3\. **Private Routes**

*   **Cart Page**:
    *   Allow users to place orders for products.
    *   Ensure the ordered quantity does not exceed the product stock.
    *   Include **product details**, **user details**, and **total price calculations**.
    *   The payment option should be cash on delivery only.
    *   Include an **Order Now** button to confirm the purchase.
*   **Dashboard (Role-Based Access)**:
    *   **Admin Dashboard**:
        *   Manage users (e.g., deactivating accounts).
        *   Manage products (CRUD).
        *   Manage orders (CRUD).
            *   Approve orders, will change the order status from "Pending" to "Shipping"
    *   **User Dashboard**:
        *   View orders.
        *   Manage profile settings (for example default shipping address).

* * *

### **UI/UX Design** (15 Marks)

*   **Responsive Design**:
    *   Ensure the platform works seamlessly on all screen sizes.
    *   Use proper alignment, typography, and intuitive layouts.
*   **Error Handling**:
    *   Show user-friendly error messages for:
        *   Invalid login credentials.
        *   Registration errors (e.g., duplicate email).
        *   Failed operations (e.g., out-of-stock products).
*   **Loading States**:
    *   Display spinners or loaders during API calls (e.g., login, data fetch).
*   **Toasts**:
    *   Notify users of important actions (e.g., "Login successful", "Order placed").

  

Inspiration for design

  

[https://www.papier.com/us/stationery/](https://www.papier.com/us/stationery/)

[https://www.muji.us/collections/stationery](https://www.muji.us/collections/stationery)

[https://bungu.store/collections/towels](https://bungu.store/collections/towels)

[https://shibuya-stationery.com/](https://shibuya-stationery.com/)
