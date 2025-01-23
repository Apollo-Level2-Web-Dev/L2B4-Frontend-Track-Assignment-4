### **Bike Shop Application Requirements**

* * *

### **Project Overview & Objective**:

Create a **Bike Shop** application with user-friendly features, secure authentication, and smooth product management. Ensure the platform is responsive, error-free, and visually appealing.

* * *

### **Main Functionalities**: 45 Marks

* * *

#### **1\. User Registration & Authentication (Role-Based)**

*   **Secure Registration and Login**:
    *   Users can register with the following fields: name, email, and password. By default, the registered user will have the "customer" role.
    *   Note: You will have to manually update a user to "admin." No need to implement a "super admin" functionality.
    *   Passwords must be securely hashed before storing in the database.
    *   Users can log in using their email and password.
*   **JWT (JSON Web Token)**:
    *   Generate a JWT token upon login for secure authentication.
    *   Store the token in **local storage** to maintain user sessions.
*   **Logout**:
    *   Clear the token from **local storage** upon logout and redirect the user to the login page.

* * *

#### **2\. Public Routes**

*   **Home Page**:
    *   **Navbar**: Include a logo, favicon, navigation items, and buttons for login/signup and other interactions.
    *   **Banner**: Highlight your platform or special offers. A carousel can be used if desired.
    *   **Featured Products**: Display up to 6 products with a "View All" button. On clicking the "View All" button, the user will be redirected to the "All Products" Page.
    *   **Extra Section**: Add relevant e-commerce content, such as testimonials or blogs.
    *   **Footer**: Include essential links, social media icons, and contact details.
*   **All Products Page**:
    *   **Search Functionality**: Allow users to search by brand, bike name, or category.
    *   **Filters**: Include options for price range, model, brand, category, and availability.
    *   **Dynamic Results**: Results should be updated based on search terms or selected filters.
    *   **Product Cards**: Show details like name, brand, model, price, and category.
    *   **"View Details"** button for each product.
*   **Product Details Page**:
    *   Display the product image and detailed information.
    *   Provide a "Buy Now" button that redirects to the checkout page.
*   **About Page**:
    *   Create an informative page about your shop and its mission. Add any other relevant details.

* * *

#### **3\. Private Routes**

*   **Checkout Page**:
    *   Users can place orders for products.
    *   Ensure the ordered quantity does not exceed the product stock.
    *   **Order Form**: Include product details, user details, total price calculation, and payment method.
    *   **Payment Integration**: Integrate SurjoPay as the payment gateway.
    *   Include an "Order Now" button to confirm the purchase.
*   **Dashboard (Role-Based Access)**:
    *   **Admin Dashboard**:
        *   Features include managing users (e.g., deactivating accounts), managing products (CRUD), and managing orders (CRUD).
    *   **User Dashboard**:
        *   Features include viewing orders and managing profile settings.
        *   Allow users to update passwords (require current password for security).

* * *

### **UI/UX Design**: 15 Marks

*   **Responsive Design**:
    *   Ensure the platform works seamlessly on all screen sizes.
    *   Use proper alignment, typography, and intuitive layouts.
*   **Error Handling**:
    *   Show user-friendly error messages for:
        *   Invalid login credentials.
        *   Registration errors (e.g., duplicate email).
        *   Failed operations (e.g., out-of-stock products).
*   **Loading States**:
    *   Display spinners or loaders during API calls, such as on login or data fetch.
*   **Toasts**:
    *   Notify users of important actions (e.g., "Login successful," "Order placed," etc.).

* * *

### **Recommendation Functionalities (Optional)**

*   **Track Order Section (Dashboard)**:

**User Side**:

*   **Track Order Status**:
    *   Display current order status (Pending, Processing, Shipped, Delivered) with a progress bar or step indicator.
    *   Show clear labels for each step in the process.
*   **Order Tracking Page**:
    *   Add a "Track My Order" page in the user dashboard.
    *   Show key order details:
        *   Order ID
        *   Product name, quantity, and price
        *   Estimated delivery date
        *   Current status

**Admin Side**:

*   **Update Order Status**:
    *   Add a dropdown in the Admin Dashboard to update order statuses (Pending, Processing, Shipped, Delivered) and a field for giving the estimated delivery date.
    *   Ensure status changes are automatically visible to users.

* * *

* * *

### **Backend Requirements**:

*   **Database**: MongoDB. Ensure schema includes:
    *   Users (with roles: customer, admin)
    *   Products (with details like name, brand, price, model, stock)
    *   Orders (with user reference, product details, total price, status)
*   **Authentication**:
    *   Implement user registration, login, JWT token generation, and logout.
    *   Secure password hashing and user session management.
*   **Product Management**:
    *   CRUD operations for products (create, read, update, delete).
*   **Order Management**:
    *   CRUD operations for orders (create, read, update, delete).
    *   Ensure stock availability before placing orders.
*   **Payment Integration**:
    *   Integrate SurjoPay for payment processing.
*   **Error Handling**:
    *   Implement consistent and user-friendly error responses for invalid login attempts, out-of-stock products, etc.
*   **Performance Optimization**:
    *   Optimize API responses and ensure smooth operation for large data loads.

* * *

### **Additional Changes**:

*   Ensure the backend API supports pagination for product listings and order retrieval.
*   Add authentication middleware to secure private routes, such as the checkout and dashboard.
