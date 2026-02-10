# 🛍️ ShopVibe - Colorful E-Commerce Website

A fully functional, vibrant e-commerce website built with **HTML, CSS, and JavaScript** only!

## ⚠️ Project Note 

This project was developed as an **AI-assisted learning project**.

The overall structure and feature ideas were generated with the help of AI, and my focus was on:
- Understanding the complete codebase
- Learning how a full e-commerce frontend works
- Exploring UI/UX patterns and user flows
- Studying state handling using JavaScript and `localStorage`
- Experimenting with styles, layouts, and logic

This repository is shared **for learning and demonstration purposes**, not as a production-ready or fully self-built system.

---
## ✨ Features

### 🎨 Design
- **Colorful & Modern UI** with gradients, animations, and smooth transitions
- **Fully Responsive** - works on mobile, tablet, and desktop
- **Dark Mode Toggle** for comfortable browsing
- **Glassmorphism** and decorative elements
- **Smooth animations** and micro-interactions

### 🛒 Shopping Features
- Browse products by category
- Advanced filtering (price, rating, category)
- Product search with auto-suggestions
- Sort products (price, rating, newest)
- Add to cart with quantity control
- Wishlist functionality
- Product detail pages with image gallery

### 💳 Checkout & Payments
- Secure checkout process
- Multiple payment methods (Card, UPI, COD)
- Coupon/discount system
- Order summary and tracking
- Free shipping on orders above ₹999

### 👤 User Features
- User registration and login
- User dashboard with order history
- Admin dashboard with analytics
- Profile management

### 📱 Pages Included
1. **Home** - Hero section, featured products, categories
2. **Shop** - Full product listing with filters
3. **Product Detail** - Detailed product view
4. **Cart** - Shopping cart management
5. **Wishlist** - Saved items
6. **Checkout** - Order placement
7. **Login/Register** - User authentication
8. **Dashboard** - User orders and profile
9. **Admin** - Admin panel with stats
10. **About, Contact, FAQ** - Information pages

## 🚀 How to Run

### Option 1: Simple Local Server (Recommended)

1. **Extract the website folder**
2. **Open with VS Code** (or any code editor)
3. **Install Live Server extension** in VS Code
4. **Right-click on `index.html`** and select "Open with Live Server"
5. Website will open at `http://localhost:5500` or similar

### Option 2: Python Server

```bash
# Navigate to the website folder
cd ecommerce

# Python 3
python -m http.server 8000

# Open browser and go to http://localhost:8000
```

### Option 3: Node.js Server

```bash
# Install http-server globally
npm install -g http-server

# Navigate to website folder
cd ecommerce

# Start server
http-server -p 8000

# Open browser and go to http://localhost:8000
```

### Option 4: Direct Open (May have limitations)

Simply double-click `index.html` - but some features may not work properly due to browser security restrictions.

## 🔐 Demo Credentials

### Admin Account
- **Email:** admin@shopvibe.com
- **Password:** admin123

### Create Your Own Account
Just click "Register" and create a new account!

## 📁 Project Structure

```
ecommerce/
├── index.html              # Home page
├── shop.html               # Products listing
├── product.html            # Product details
├── cart.html               # Shopping cart
├── wishlist.html           # Wishlist
├── checkout.html           # Checkout page
├── login.html              # Login page
├── register.html           # Registration
├── dashboard.html          # User dashboard
├── admin.html              # Admin panel
├── about.html              # About page
├── contact.html            # Contact page
├── faq.html                # FAQ page
├── css/
│   ├── style.css           # Main styles
│   ├── shop.css            # Shop page styles
│   ├── cart.css            # Cart styles
│   ├── checkout.css        # Checkout styles
│   ├── product.css         # Product detail styles
│   └── auth.css            # Auth pages styles
└── js/
    ├── data.js             # Product & user data
    ├── utils.js            # Utility functions
    ├── main.js             # Home page logic
    ├── shop.js             # Shop page logic
    ├── cart.js             # Cart logic
    ├── checkout.js         # Checkout logic
    ├── product.js          # Product detail logic
    └── auth.js             # Authentication logic
```

## 💡 Features Breakdown

### LocalStorage Database
All data is stored in browser's localStorage:
- **Products** - 30 sample products across 6 categories
- **Cart** - Persists between sessions
- **Wishlist** - Saved favorite items
- **Orders** - Order history
- **Users** - User accounts
- **Coupons** - Discount codes

### Available Coupons
- **FIRST50** - 50% off on orders above ₹1000
- **SAVE200** - ₹200 off on orders above ₹2000
- **WELCOME10** - 10% off on orders above ₹500
- **MEGA30** - 30% off on orders above ₹1500

### Categories
1. Electronics (Headphones, Smartwatch, Laptop Stand, etc.)
2. Fashion (Jackets, T-shirts, Sunglasses, Wallets)
3. Home & Living (Diffusers, Wall Art, Pillows, Lights)
4. Beauty (Skincare, Makeup Brushes, Hair Tools)
5. Sports (Yoga Mats, Dumbbells, Resistance Bands)
6. Books (Programming, AI/ML, Web Development)

## 🎯 Key Functionalities

### Shopping Flow
1. Browse products on home page or shop
2. Use filters to find products
3. Click product to see details
4. Add to cart or wishlist
5. Go to cart and review items
6. Apply coupon code (optional)
7. Proceed to checkout
8. Fill shipping details
9. Select payment method
10. Place order
11. View order in dashboard

### Admin Features
- View total products, orders, revenue, users
- See recent orders
- Monitor business stats

## 🎨 Color Scheme

The website uses a vibrant color palette:
- **Primary:** #FF6B6B (Coral Red)
- **Secondary:** #4ECDC4 (Turquoise)
- **Accent:** #FFE66D (Yellow)
- **Purple:** #A06CD5
- **Blue:** #6C5CE7
- **Pink:** #FD79A8
- **Green:** #55EFC4

## 📱 Responsive Breakpoints

- **Desktop:** > 968px
- **Tablet:** 768px - 968px
- **Mobile:** < 768px

## 🔧 Customization

### Add More Products
Edit `js/data.js` and add products to the `products` array:

```javascript
{
    id: 31,
    name: "Your Product Name",
    category: "electronics",
    price: 1999,
    originalPrice: 3999,
    image: "https://your-image-url.jpg",
    rating: 4.5,
    reviews: 100,
    description: "Product description",
    stock: 50,
    featured: true,
    badge: "New"
}
```

### Change Colors
Edit CSS variables in `css/style.css`:

```css
:root {
    --primary: #YOUR_COLOR;
    --secondary: #YOUR_COLOR;
    /* ... */
}
```

### Modify Payment Methods
Edit the payment methods section in `checkout.html`

## ⚡ Performance

- **Fast Loading:** Optimized CSS and JS
- **Smooth Animations:** GPU-accelerated transitions
- **Efficient:** No heavy frameworks
- **SEO-Friendly:** Semantic HTML

## 🌟 Special Features

1. **Toast Notifications** - Beautiful success messages
2. **Skeleton Loading** - Smooth content loading
3. **Lazy Loading** - Images load as needed
4. **Smooth Scrolling** - Anchor links scroll smoothly
5. **Form Validation** - Real-time input validation
6. **Auto-save** - Cart and wishlist persist automatically

## 🐛 Troubleshooting

### Products not showing?
- Check browser console for errors
- Clear localStorage and refresh: `localStorage.clear()`

### Cart not working?
- Enable localStorage in browser settings
- Check if cookies are enabled

### Images not loading?
- Check internet connection (using Unsplash CDN)
- Some images may take time to load

## 📝 Notes

- This is a **frontend-only** demo website
- Payments are **simulated** (not real transactions)
- Data is stored in **browser localStorage**
- No backend server required
- Perfect for learning and portfolio projects

## 🎓 Learning Purposes

Great for learning:
- HTML5 semantic markup
- CSS Grid & Flexbox
- Vanilla JavaScript
- LocalStorage API
- Responsive design
- UI/UX design patterns
- E-commerce workflows

## 💻 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ⚠️ IE11 (limited support)

## 📄 License

This is a demo project for educational purposes. Free to use and modify!

## 🤝 Contributing

Feel free to fork, modify, and use for your projects!

## 💬 Support

For any questions or issues, feel free to reach out!

---

**Made with ❤️ for learning HTML, CSS & JavaScript**

**Happy Shopping! 🛍️**
