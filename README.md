# Django Shopping Cart System (Based on GeeksforGeeks Tutorial)

## Overview
This project is a simple shopping cart system built using Django, following the tutorial from GeeksforGeeks. It demonstrates how to create and manage a cart using Django's built-in database without relying on JavaScript, AJAX, or JSON-based storage. The approach focuses on simplicity while utilizing Django's session management and model-based cart storage.

## Features
- Add items to the cart.
- View the cart with item details and total price.
- Remove items from the cart.
- Persistent cart storage using Django's default database.

## How the Program Works
1. **Models:** The system defines models for `Product` and `Cart`. The `Product` model stores item details, while the `Cart` model keeps track of items added to the user's cart.
2. **Views:** Django views handle adding items, viewing the cart, and removing items. The logic is handled on the backend without JavaScript.
3. **Templates:** HTML templates render the product list and cart page, using Django’s template language to display dynamic data.
4. **URLs:** The project includes URL routes for the main product listing, cart view, and cart modifications.
5. **Database Storage:** Instead of using JavaScript-based local storage or AJAX calls, the cart items are stored in the database, ensuring persistence across sessions.

## Installation & Setup
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <project_directory>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run migrations to set up the database:
   ```bash
   python manage.py migrate
   ```
4. Start the Django development server:
   ```bash
   python manage.py runserver
   ```
5. Access the application at `http://127.0.0.1:8000/`.

## Considerations & Future Improvements
- **Database vs. Sessions:** Using Django’s default database for cart storage works well, but an alternative approach is to store cart data in Django sessions for lighter storage.
- **Enhancing User Experience:** Implementing JavaScript for live cart updates without page reloads can improve usability.
- **Payment Integration:** Extending the system to include checkout and payment processing can make it more complete.

This project serves as a fundamental introduction to shopping cart systems in Django, providing a solid base for further improvements and enhancements.

