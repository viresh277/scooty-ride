# 🛵 ScootyRide - Vehicle Rental Platform

A modern, responsive vehicle rental platform built with React and Tailwind CSS. Features a sleek interface for browsing, filtering, and booking scooters with an intuitive multi-step booking process.
<img width="955" height="451" alt="image" src="https://github.com/user-attachments/assets/bbd7db34-a7c7-4ad5-b2e0-440d8f5b773b" />

![Uploading image.png…]()


## ✨ Features

### 🎯 Core Functionality
- **Vehicle Browsing** - Explore our premium fleet with detailed specifications
- **Smart Search** - Find vehicles by name, category, or features
- **Advanced Filtering** - Filter by category, price, rating, and availability
- **Multi-step Booking** - Streamlined 4-step booking process
- **Favorites System** - Save and manage your preferred vehicles
- **Real-time Availability** - Live availability status for all vehicles

### 🎨 Modern UI/UX
- **Responsive Design** - Optimized for mobile, tablet, and desktop
- **Contemporary Aesthetics** - Gradient backgrounds, glassmorphism effects
- **Smooth Animations** - Hover effects, transitions, and micro-interactions
- **Intuitive Navigation** - Mobile-first design with collapsible menu
- **Visual Feedback** - Loading states, success indicators, and error handling

### 📱 Mobile Experience
- Touch-friendly interface
- Swipe gestures support
- Optimized loading times
- Progressive web app ready

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn package manager

### Installation

1. **Clone or download the project**
```bash
git clone <your-repo-url>
cd scootyride
```

2. **Install dependencies**
```bash
npm install
# or
yarn install
```

3. **Install required packages**
```bash
npm install lucide-react
```

4. **Set up Tailwind CSS**

**Option A: CDN (Quick Setup)**
Add this to your `public/index.html` in the `<head>` section:
```html
<script src="https://cdn.tailwindcss.com"></script>
```

**Option B: Full Installation (Recommended)**
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

Configure `tailwind.config.js`:
```javascript
module.exports = {
  content: ["./src/**/*.{js,jsx,ts,tsx}"],
  theme: { extend: {} },
  plugins: [],
}
```

Add to `src/index.css`:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

5. **Replace your App.js content**
Copy the ScootyRide component code to your `src/App.js`

6. **Start the development server**
```bash
npm start
```

Visit `http://localhost:3000` to see your application! 🎉

## 📖 Usage Guide

### 🏠 Homepage
- **Hero Section**: Eye-catching gradient background with search functionality
- **Feature Cards**: Highlight key benefits (Insurance, Instant Booking, 24/7 Support)
- **Navigation**: Responsive header with mobile hamburger menu

### 🛵 Vehicle Fleet
- **Search Bar**: Find vehicles by name or specifications
- **Filter Panel**: Filter by category, price range, rating, and availability
- **Vehicle Cards**: Detailed information including:
  - High-quality images
  - Ratings and reviews
  - Key features and specifications
  - Pricing and availability status
  - Favorite toggle functionality

### 📅 Booking Process

**Step 1: Duration Selection**
- Choose pickup and return dates
- Select time slots
- View pricing calculation

**Step 2: Personal Details**
- Enter contact information
- Provide driving license details
- Add address information

**Step 3: Payment**
- Choose payment method (UPI, Card, Pay at Pickup)
- Review booking summary
- Confirm total amount

**Step 4: Confirmation**
- Receive booking confirmation
- Get unique booking ID
- Email confirmation sent

## 🎨 Customization

### 🎯 Vehicle Data
Modify the `vehicles` array in the component to add your own fleet:

```javascript
const vehicles = [
  {
    id: 1,
    name: "Your Vehicle Name",
    category: "scooter" | "electric",
    price: 299,
    rating: 4.8,
    reviews: 124,
    image: "https://your-image-url.jpg",
    features: ["Feature 1", "Feature 2", "Feature 3"],
    range: "60km",
    topSpeed: "60km/h",
    available: true
  },
  // Add more vehicles...
];
```

### 🎨 Styling
The platform uses Tailwind CSS utility classes. Key design elements:

- **Primary Color**: Blue (blue-500, blue-600)
- **Secondary Color**: Purple (purple-600)
- **Success Color**: Green (green-500)
- **Background**: Gray scales (gray-50, gray-100)

### 🔧 Configuration
Update company information in the header and footer:

```javascript
// Header brand
<h1 className="text-xl font-bold text-gray-900">Your Brand</h1>

// Footer contact info
<li>📱 Your Phone Number</li>
<li>✉️ your-email@domain.com</li>
<li>📍 Your Location</li>
```

## 📁 Project Structure

```
src/
├── App.js              # Main component with all functionality
├── index.js            # React entry point
├── index.css           # Global styles (Tailwind imports)
└── ...

public/
├── index.html          # HTML template (add Tailwind CDN here)
└── ...
```

## 🛠️ Tech Stack

- **Frontend Framework**: React 18
- **Styling**: Tailwind CSS 3.x
- **Icons**: Lucide React
- **State Management**: React Hooks (useState)
- **Build Tool**: Create React App

## 🌟 Key Components

### Main Features
- **Responsive Header**: Navigation with mobile menu
- **Hero Section**: Search functionality with gradient background
- **Features Section**: Service highlights with icons
- **Vehicle Grid**: Filterable and searchable vehicle catalog
- **Booking Modal**: Multi-step booking process
- **Footer**: Contact information and links

### Interactive Elements
- Search and filter functionality
- Favorite vehicles toggle
- Multi-step form wizard
- Responsive modal dialogs
- Mobile-optimized navigation

## 🔄 Future Enhancements

- [ ] User authentication system
- [ ] Real-time booking availability
- [ ] Payment gateway integration
- [ ] GPS location services
- [ ] Push notifications
- [ ] Admin dashboard
- [ ] Vehicle tracking
- [ ] Review and rating system
- [ ] Loyalty program
- [ ] Multi-language support

## 📱 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Troubleshooting

### Common Issues

**Styling not appearing:**
- Ensure Tailwind CSS is properly installed
- Check that the CDN link is in your `index.html`
- Restart your development server

**Icons not showing:**
- Install lucide-react: `npm install lucide-react`
- Ensure proper import statements

**Mobile view issues:**
- Check viewport meta tag in `index.html`
- Verify responsive breakpoints in Tailwind classes

### Getting Help

- 📧 **Email**: support@scootyride.com
- 💬 **Issues**: [GitHub Issues](https://github.com/your-username/scootyride/issues)
- 📖 **Documentation**: [Tailwind CSS Docs](https://tailwindcss.com/docs)

## 🎉 Deployment

### Quick Deployment Options

**Netlify:**
```bash
npm run build
# Drag and drop the build folder to Netlify
```

**Vercel:**
```bash
npx vercel
```

**GitHub Pages:**
```bash
npm install --save-dev gh-pages
npm run build
npm run deploy
```

---

**Made with ❤️ using React and Tailwind CSS**

*Happy Coding! 🚀*
