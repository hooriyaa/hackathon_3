## ✨Comforty: E-Commerce Platform for Sofas and Chairs

## Overview:
Comforty is an e-commerce platform specializing in offering a wide variety of sofas and chairs. The platform is built using Sanity CMS as the backend for managing product data and integrates third-party APIs for shipping and payments. 
Below is a detailed breakdown of the project features, architecture, and workflow.

## Features:
## Sanity CMS Integration:
-Acts as the backend to store and manage:

• Product Data: ID, Name, Old Price, New Price, Stock, Category, Description, Image, Rating.

• Categories: Sofas, Chairs, Stools.

• Order Records: Tracks user orders and purchase history.

## Responsive Design:
-Fully responsive user interface for all pages, ensuring a seamless experience across various devices and screen sizes.

## Third-Party API Integration:
•ShipEngine: Used for calculating shipping rates and tracking orders.

•Stripe: Used for secure payment processing.

•Clerk: Used for user authentication and profile management.

## User Interface Workflow:

## Home Page (localhost:3000/)
•Displays a list of products fetched from Sanity CMS.

•Each product includes a name, image, price, and rating.

•Users can click on a product to navigate to its detail page.

## Product Detail Page (localhost:3000/product/:id)

•Displays detailed information about a specific product, including:

•Name, Image, Old Price, New Price, Description, Stock, and Rating.

•Allows users to add the product to the cart or wishlist.

## Cart (localhost:3000/cart)

•Lists all added products with their quantity and total price.

•Users can modify quantities or remove products from the cart.

•Users must be signed in to proceed to payment.

•Collects shipping information and integrates ShipEngine to calculate shipping rates.

•Users must be signed in to proceed to payment.

## Payment Page (localhost:3000/cart/payment)

•Processes payments securely using Stripe.

•Users must be signed in to complete the payment.

## Shipment Page (localhost:3000/shipment)

•Displays shipping details and allows users to confirm their shipment information.

•Provides an option to track the order using ShipEngine.

## Wishlist (localhost:3000/wishlist)

•Displays products saved by the user for future reference.

•Users can move items from the wishlist to the cart.

## User Authentication (localhost:3000/login)

•Provides secure user authentication using Clerk.

•Users can sign up, log in, and manage their profiles.

✨## Application Workflow:
## Home Page:
•Displays a responsive product listing with advanced category filters.

•Users can browse sofas, chairs, and stools.

## Product Detail Page:

•Shows detailed product information, including reviews and ratings.

•Users can add products to the cart or wishlist.

## Cart:

•Displays selected products with their quantities and total price.

•Users must be signed in to proceed to payment.

## Checkout:

•Collects shipping details and calculates shipping rates using ShipEngine.

•Users must be signed in to proceed to payment.

## Payment:

•Processes payments securely using Stripe.

•Users must be signed in to complete the payment.


## Shipment Page:

•Displays shipping details and allows users to confirm their shipment information.

•Provides an option to track the order using ShipEngine.

## Order Confirmation:

•Displays a success message with order details and shipping information.


**Product Data Structure**
Managed via Sanity CMS:

**{
  "ID": "string",
  "Name": "string",
  "Old Price": "number",
  "New Price": "number",
  "Stock": "number",
  "Category": "string (sofas, chairs, stools)",
  "Description": "string",
  "Image": "string (URL)",
  "Rating": "number (1-5)"
}
**


✨## Technologies Used
•Frontend: React.js, Tailwind CSS
•Backend: Sanity CMS
•Authentication: Clerk
•Shipping: ShipEngine
•Payments: Stripe


## Performance Testing: Lighthouse


## Conclusion
**Comforty is a fully functional e-commerce platform designed to provide a seamless shopping experience for users looking to purchase high-quality sofas and chairs. With robust backend integration, responsive design, and secure payment processing, Comforty is ready for real-world deployment. Users must be signed in to proceed to payment, ensuring a secure and personalized shopping experience.**
