# Assignment 4

## Project Overview:

You are tasked with implementing a responsive website based on the provided requirements. The website should include the following sections: Navbar, Header, Our Services, Event Items, Gallery, Pricing, Review, Recent Events, and Footer. If the Figma file includes extra sections, make sure to include them in your website too. This way, you're building exactly what the design suggests.

## **Frontend Requirements**

---

1. **User Registration & Authentication**
    - Implement role-based authentication (e.g., user, admin).
    - Provide smooth user registration and login functionality.
2. **Routing (Other Pages)**
    - **Public Routes:**
        - **Home Page**: Display an overview of the platform.
        - **All Products Page**: Showcase all available bicycles with filtering and sorting options.
        - **Product Details Page**: Display detailed information about a specific bicycle.
        - **About Us Page**: Provide information about the platform/company.
    - **Private Routes:**
        - **Checkout Page**: Accessible to authenticated users for placing orders.
        - **Dashboard (Role-Based Access):**
            - **User Role:** View order history and account details.
            - **Admin Role:** Manage products, view orders, and oversee platform activities.
3. **UI/UX Design**
    - Ensure an intuitive, responsive, and visually appealing interface.
    - Prioritize user-friendliness across all device sizes.
    - Design Guideline: [Design_Guideline - Google Docs](https://docs.google.com/document/d/1mMxoWIGJNKDtnbCHAeJzR4Gdi6IZ393G85eLdt6NDns/edit?tab=t.0)

## **Backend Requirements (Module Pattern):**

- **Database:** Use MongoDB with a schema including:
    - Users (defined roles: user, admin)
    - products (with attributes like name, brand, price, model, stock)
    - Orders (linked to user, product details, total price, status)
- **Authentication:**
    - Implement user registration, login, JWT token management, and logout.
    - Ensure secure password hashing and user session handling.
- **Product Management:**
    - Implement CRUD operations for bicycles (create, read, update, delete).
- **Order Management:**
    - Execute CRUD operations for orders (create, read, update, delete), ensuring stock levels before orders are placed.
- **Payment Integration:**
    - Utilize SurjoPay/AmaarPay/SSLCommerz/Stripe or any other payment gateway for payment processing.
- **Error Handling:**
    - Establish consistent, user-friendly error messaging for invalid login attempts, out-of-stock bicycles, etc.
- **Additional Changes:**
    - Ensure backend APIs support pagination for product listings and order retrieval.
    - Add authentication middleware to protect private routes, including checkout and the dashboard

`You can use any existing backend if you have developed it earlier or create a new version modifying from the existing older one.`

## Technical Requirements:

1. **API Integration:**
    - Fetch service and event data from a RESTful API.
    - Utilize RTK Query for efficient data management.
2. **Technology Stack:**
    - TypeScript
    - React
    - Redux
    - Node / Express

## **Submission Guidelines:**

- Submit a well-documented codebase with clear comments.
- Make sure to add a README file that explains how to set up and use the application. In the README, include details like the project name, live URL, features, technology used, and other important information. Try to make it look professional by doing some research and making it appealing.

## Submission:

- Provide the GitHub repository links of the front end and back end and ensure there is a README file with explicit instructions for running the application locally.
- Live deployment link
- Provide Admin Credentials (email & password)
- Submit a demo video showcasing the functionality of the Inventory Management Dashboard.

## Assignment Number based on the Last Digit of PH Student ID:

| Last Digit of PH Student ID | Assignment Number (Design No) |
| --- | --- |
| 0, 1 | [1](./1-Book-Shop-Assignment-Requirement.md) |
| 2, 3 | [2](./2-Bike-Shop-Assignment-Requirement.md) |
| 4, 5 | [3](./3-Car-Shop-Assignment-Requirement.md) |
| 6, 7 | [4](./4-Bi-Cycle-store-Assignment-Requirement.md) |
| 8, 9 | [5](./5-Stationery-Shop-Assignment-Requirement.md) |

## **Deadline:**

- 60 marks: January 29, 2025 11.59 PM
- 50 marks: January 30, 2025 11.59 PM
- 30 marks: After January 31, 2025 11.59 PM

## Important Note:

Plagiarism will not be tolerated. Ensure that the code you submit is your own work. Any instances of plagiarism will result in 0 Marks.

Good luck with your assignment! If you have any questions, feel free to reach out for clarification.
