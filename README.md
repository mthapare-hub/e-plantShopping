# e-plantShopping

## Project Name
**Paradise Nursery: e-plantShopping**

## Overview
e-plantShopping is a React e-commerce front end for Paradise Nursery, an online houseplant shop ("Where Green Meets Serenity"). The app is built with React and Redux Toolkit and bundled with Vite.

## Current Status
This repository is based on a starter template and is a work in progress.

**Implemented**
- Landing page with a "Welcome To Paradise Nursery" heading, a **Get Started** button, and an About Us section (`App.jsx`, `AboutUs.jsx`)
- Navigation bar with the Paradise Nursery logo, a **Plants** link, and a cart icon (`ProductList.jsx`)
- Plant catalog data: 5 categories with 6 plants each, including name, image, description, and price
  - Air Purifying Plants
  - Aromatic Fragrant Plants
  - Insect Repellent Plants
  - Medicinal Plants
  - Low Maintenance Plants
- Redux store configured with a `cart` slice (`store.js`)
- Cart page layout with quantity buttons, Delete, Continue Shopping, and Checkout buttons (`CartItem.jsx`)

**Still to be built**
- Rendering the plant catalog in the product grid
- Cart logic in `CartSlice.jsx`: `addItem`, `removeItem`, `updateQuantity`
- Cart total and per-item cost calculations
- Cart item count shown on the cart icon
- Working Continue Shopping and Checkout actions

## Tech Stack
- React 18
- Redux Toolkit and React-Redux
- Vite 5
- ESLint

## Getting Started

### Prerequisites
- Node.js and npm

### Installation
```bash
git clone https://github.com/mthapare-hub/e-plantShopping.git
cd e-plantShopping
npm install
```

### Run locally
```bash
npm run dev
```
Open the URL shown in the terminal. Because `vite.config.js` sets `base: "/shoppingreact"`, the app may be served under that path (for example `http://localhost:5173/shoppingreact`).

### Other scripts
```bash
npm run build    # production build
npm run preview  # build and preview
npm run lint     # run ESLint
```

## Project Structure
```
e-plantShopping/
├── public/
├── src/
│   ├── App.jsx          # Landing page and app shell
│   ├── AboutUs.jsx      # About Us section
│   ├── ProductList.jsx  # Navbar and plant catalog data
│   ├── CartItem.jsx     # Shopping cart view
│   ├── CartSlice.jsx    # Redux cart slice
│   ├── store.js         # Redux store
│   └── main.jsx         # Entry point
├── index.html
├── package.json
└── vite.config.js
```

## License
See the [LICENSE](LICENSE) file in this repository.