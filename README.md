# UCLAN PHP SHOP - Assignment 2

Extending from Assignment 1 which utilises Javascript to parse hardcoded data via manipulating the DOM, I have developed this source which utilises MySQL Backend DB alongside with PHP to create a professional shop matching UCLan's corporate theming. I'd like to thank you for taking time outside of your daily routine to review my source due to my mitigating circumstances.

## Table of Contents
- [Features](#features)
- [Login Functionality](#login-functionality)
- [Live Offers](#live-offers)
- [Product Management](#product-management)
- [User Registration](#user-registration)
- [Product Reviews](#product-reviews)
- [Responsive Design](#responsive-design)
- [Advanced Search](#advanced-search)
- [Checkout Mechanism](#checkout-mechanism)
- [Custom 404 Error Page](#custom-404-error-page)
- [Security](#security)
- [Additional Functionality](#additional-functionality)

## Features

### Login Functionality
- Users can create accounts and log in securely (Faced with reCaptcha challenge)
- Only logged-in users can access the checkout process as when a logged-out user attempts to add anything to their cart they are forced to log-in.
- Personalised greetings are displayed to logged-in users with their full-name.

### Live Offers
- Live offers are retrieved from the database and displayed on the homepage.
- Offers are visible to all users, whether logged in or not - GRAD2022 coupon should work directly with the Stripe Payment Processor.

### Product Management
- Products are stored in a MySQL database and retrieved dynamically.
- Products are categorised, allowing users to browse specific categories.
- Clicking on a product reveals more information on a dedicated product page (item page which is a individual page relating to the product, which also includes reviews on the product by users).

### User Registration
- Users can sign up and create accounts. (Recaptcha Integration and CSRF)
- Registration includes fields for necessary user information.

### Product Reviews
- Users can submit reviews for products.
- Reviews include a title, description, and rating.
- Product reviews are displayed on the product information page.

### Responsive Design
- The application is designed to be responsive, adapting to different screen sizes.
- Dynamic content is presented in a user-friendly manner across devices.

### Advanced Search
- Advanced search functionality allows users to search for products based on specific criteria (Category, name and other values)
- The search utilizes Javascript, not MYSQL's LIKE criteria, as its just not necessary. 

### Checkout Mechanism
- Logged-in users can check out their shopping cart.
- Stripe Test Environment Utilised - Use test card 4242 4242 4242 4242 mm/yy cvv (for Approval)
- Orders are added to the database, and a success message is displayed.
- The shopping cart is emptied after a successful checkout (session with all the product id's in the cart id destroyed)

### Custom 404 Error Page
- A custom 404 error page is provided for handling invalid URLs (using .htaccess)

### Security
- Passwords are securely stored using bcrypt hashing and salting.
- User authentication and session management are implemented to ensure secure access.

### Additional Functionality
- The application includes extended functionality and presentation beyond the required criteria.
- The design and structure of the web application demonstrate best practices in web development.
- Recaptcha
- CSRF
- Stripe Test Environment
- My Orders Page (With Review Functionality)


For any enquiries, please contact Spencer Schotel at sschotel@uclan.ac.uk (G20993503)
