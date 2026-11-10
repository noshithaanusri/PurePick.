# PurePick – Project Review 2

PurePick is a grocery shopping demo built with **React + Vite**. It includes separate Customer and Admin modules, Local Storage authentication, shopping cart, checkout, order tracking/status management and inventory management. Product/category/hero pictures from the supplied project are retained in `public/images`.

## Run locally
1. Install Node.js (LTS).
2. Extract this ZIP and open the `PurePick_Review2_ReactVite` folder in VS Code.
3. Open Terminal and run:
   ```bash
   npm install
   npm run dev
   ```
4. Open the localhost URL printed by Vite.

## Demo login
- **Admin:** `admin@purepick.com`
- **Password:** `admin123`
- Customer: use **Sign up** to create an account, then log in as Customer.

## Deploy to Vercel
1. Create a GitHub repository and upload/push all files in this folder (including `package.json`, `src`, `public`, `vite.config.js`, and `vercel.json`).
2. In Vercel choose **Add New → Project**, import the GitHub repository.
3. Framework preset: **Vite**. Build command: `npm run build`. Output directory: `dist`.
4. Click Deploy. `vercel.json` includes an SPA rewrite so routes work on refresh.
5. Test the deployed URL: sign up/login as customer, add products, place an order, then log out and login as admin to update the order and manage inventory.
6. Add your GitHub repository URL and Vercel deployment URL to your review presentation.

## Git commands
```bash
git init
git add .
git commit -m "PurePick React Vite review project"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

## Modules
- **Customer:** signup/login, browse/search/filter products, cart, delivery details, place/cancel orders, view order history.
- **Admin:** protected admin login, dashboard statistics, view all customer orders, update order status, add/delete inventory products.

## Important demo limitation
Authentication and project data use browser Local Storage as required for this academic demo. This is not production-grade security: credentials and data are stored in the browser and are not shared across different devices/browsers. Use a backend/database and hashed passwords before real-world deployment. The admin demo credentials are visible in this README for review purposes.
