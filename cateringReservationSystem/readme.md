# Catering Reservation and Ordering System

This project is a web-based catering reservation and food ordering system built with HTML, CSS, and JavaScript, using Firebase for authentication, real-time database, and storage.

## Features

- **User Registration & Login:** Users and admins can register and log in securely.
- **Admin Panel:** Admins can add, view, and delete food items, and view orders placed for their services.
- **User Interface:** Users can browse food items, add them to a cart, place orders, and view their profile.
- **Order Management:** Orders are tracked and displayed for both users and admins.
- **Firebase Integration:** Uses Firebase Authentication, Realtime Database, and Storage for backend services.

## Project Structure

```
public/
  ├── index.html              # Home page
  ├── login.html              # Login selection (User/Admin)
  ├── register.html           # Registration selection (User/Admin)
  ├── user_login.html         # User login form
  ├── user_register.html      # User registration form
  ├── user_IF.html            # User dashboard (browse food, cart, profile)
  ├── user_profile.html       # User profile page
  ├── cart.html               # User cart and order placement
  ├── admin_login.html        # Admin login form
  ├── admin_register.html     # Admin registration form
  ├── admin_IF.html           # Admin dashboard
  ├── add_product.html        # Admin: Add food item
  ├── display.html            # Admin: View and delete food items
  ├── view_order.html         # Admin: View orders for their service
  ├── *.css                   # Stylesheets for each page
  └── images/                 # Image assets (not included in repo)
firebase.json                 # Firebase hosting configuration
.firebaserc                   # Firebase project alias
.gitignore                    # Git ignore rules
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (for Firebase CLI)
- [Firebase CLI](https://firebase.google.com/docs/cli)

### Setup

1. **Clone the repository:**

   ```sh
   git clone <your-repo-url>
   cd cateringReservationSystem
   ```

2. **Install Firebase CLI (if not already):**

   ```sh
   npm install -g firebase-tools
   ```

3. **Firebase Configuration:**

   - The project is already configured for Firebase Hosting and Realtime Database.
   - If you want to use your own Firebase project, update the Firebase config in all HTML files.

4. **Serve Locally:**

   ```sh
   firebase serve
   ```

   or

   ```sh
   firebase emulators:start
   ```

5. **Deploy to Firebase Hosting:**
   ```sh
   firebase deploy
   ```

## Usage

- Visit the home page (`index.html`) to get started.
- Register as a user or admin.
- Users can browse food items, add to cart, and place orders.
- Admins can add food items, view/delete their products, and see orders placed for their service.

## File Reference

- **Authentication:**
  - User: [`public/user_login.html`](public/user_login.html), [`public/user_register.html`](public/user_register.html)
  - Admin: [`public/admin_login.html`](public/admin_login.html), [`public/admin_register.html`](public/admin_register.html)
- **Admin Dashboard:**
  - [`public/admin_IF.html`](public/admin_IF.html)
- **User Dashboard:**
  - [`public/user_IF.html`](public/user_IF.html)
- **Order Management:**
  - User Cart: [`public/cart.html`](public/cart.html)
  - Admin Orders: [`public/view_order.html`](public/view_order.html)
- **Food Item Management:**
  - Add: [`public/add_product.html`](public/add_product.html)
  - View/Delete: [`public/display.html`](public/display.html)
- **Profile:**
  - [`public/user_profile.html`](public/user_profile.html)

## Customization

- Update Firebase configuration in each HTML file to use your own Firebase project.
- Add images to the `public/images/` directory for backgrounds and food items.

## License

This project is for educational purposes.

---

**Note:**

- Make sure to secure your Firebase rules for production.
- Do not commit sensitive information (like API keys) to public repositories.

## Hosting URL

- https://catering-reservation-sys-7277d.web.app
