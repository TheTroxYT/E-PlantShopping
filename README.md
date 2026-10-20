# e-plantShopping — Paradise Nursery Shopping Application

## Project Overview
**Paradise Nursery** (`e-plantShopping`) is a dynamic React and Redux e-commerce web application built for an online houseplant shop. Users can explore a curated catalog of houseplants organized by category, view plant descriptions and pricing, add items to an interactive shopping cart, and manage item quantities with real-time cost calculations.

## Key Features
- **Landing Page (`App.jsx` & `App.css`)**: Welcomes visitors with a full-screen botanical greenhouse background image, company tagline (*"Where Green Meets Serenity"*), an integrated **About Us** overview, and a **Get Started** button that transitions smoothly to the product catalog.
- **About Us (`AboutUs.jsx`)**: Presents Paradise Nursery's mission, commitment to sustainable plant care, and service overview.
- **Product Listing (`ProductList.jsx`)**:
  - Displays **18 unique houseplants** grouped into **3 categories** (*Air Purifying Plants*, *Aromatic Fragrant Plants*, and *Low Maintenance Plants* — 6 plants per category).
  - Each plant card displays a thumbnail image, name, description, unit price, and an **Add to Cart** button.
  - Clicking **Add to Cart** dispatches the `addItem` Redux action, disables the button (`Added to Cart`), and increments the dynamic cart badge counter in the navigation bar.
  - Persistent navigation bar with links to **Home**, **Plants**, and **Cart**.
- **Redux State Management (`CartSlice.jsx`)**:
  - Built with `@reduxjs/toolkit` (`createSlice`) managing `state.items`.
  - Reducers: `addItem`, `removeItem`, and `updateQuantity`.
- **Shopping Cart (`CartItem.jsx`)**:
  - Displays the overall **Total Cart Amount** across all selected plants.
  - Shows each cart item's thumbnail, name, unit price, quantity controls (`+` and `-`), calculated item subtotal, and a **Delete** button.
  - Includes a **Continue Shopping** button returning to the plant listing and a **Checkout** button displaying a *"Coming Soon"* notification.

## Repository File Structure & Submission URLs
Replace `<your-username>` with your GitHub username when submitting Tasks 1–7:
- **Task 1 (`README.md`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/README.md`
- **Task 2 (`AboutUs.jsx`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/src/AboutUs.jsx`
- **Task 3 (`App.css`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/src/App.css`
- **Task 4 (`App.jsx`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/src/App.jsx`
- **Task 5 (`CartSlice.jsx`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/src/CartSlice.jsx`
- **Task 6 (`ProductList.jsx`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/src/ProductList.jsx`
- **Task 7 (`CartItem.jsx`)**: `https://github.com/<your-username>/e-plantShopping/blob/main/src/CartItem.jsx`

## Getting Started Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/e-plantShopping.git
   cd e-plantShopping
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Launch the development server:
   ```bash
   npm run dev
   ```
