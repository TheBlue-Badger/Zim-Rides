# Boss Yellow Taxi, Logistics Platform

## 📌 Overview
**Boss Yellow Taxi** is a modern, responsive web application I engineered for a premium door-to door vehicle transport, airport transfer, charter, and delivery service in Zimbabwe (Direct Calls / WhatsApp: **+263 77 255 0223**). Built with vanilla HTML5, CSS 3, and JavaScript, the platform offers a sleek, dynamic user experience featuring micro  animations, interactive booking management, smooth navigation, and optimized visual showcases.

---

## 🛠️ Tech Stack

- **Frontend Core:** HTML5, CSS3, JavaScript 
- **Styling Architecture:** Modern CSS Grid & Flexbox, Custom Properties (`:root` variables), Dark Glassmorphic Design System
- **APIs & Web Interfaces:** DOM Manipulation API, Intersection Observer API, `requestAnimationFrame` for performance-optimized mathematical easing
- **Design & UX:** Responsive Mobile Navigation with scroll locking, Smooth Anchor Scrolling, Dynamic CSS Glassmorphism
- **Asset Management:** Structured media asset architecture (`Images/`, `assets/`)

---

## ⚙️ Key Features & Technical Details

### 🎨 Scroll-Aware Dynamic Navigation
- **Sticky & Reactive Header:** Listens for scroll position (`window.scrollY > 60`) using passive event listeners for high FPS performance, toggling background glassmorphism dynamically.
- **Active Section Tracker:** Dynamically highlights header navigation items as the user scrolls past corresponding section boundaries (`section[id]`).

### ⚡ High-Performance Intersection Observer Animations
- **Scroll Reveals:** Employs the `Intersection Observer API` to trigger fluid fade and slide animations (`.reveal`) when elements enter the viewport threshold, bypassing expensive legacy scroll listener loops.
- **Mathematical Numerical Counters:** Stat counters utilize `requestAnimationFrame` with a custom cubic ease  out function (`1 - Math.pow(1 - progress, 3)`) to smoothly animate figures upon scroll reveal

### 📋 Interactive Booking Engine & Form Controller
- Integrated booking form controller (`app.js`) handling submission events, state transitions, client-side validation, user feedback feedback UI display, and automated reset timers.

###📱 Responsive Mobile-First Design
- Custom responsive navigation menu with animated hamburger toggles and dynamic body overflow lock (`overflow: hidden`) to deliver a native app-like experience on mobile screens.

---

## 📁 Project Structure

```
car-carrier-website/
index.html        # Main semantic markup (Hero, About, Services, Specs, Booking)
 style.css         # Design system tokens, Glassmorphism, animations, responsive queries
 app.js            # Modular application controller (Observers, header logic, counters)
 Images/           # High resolution vehicle media and showcases
 assets/           # Supporting branding assets and icons
```

---

## 🚀 How to Run Locally

### Prerequisites
No external build tools or backend dependencies are required. Any modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari) can run the project directly.

### Step-by-Step Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/TheBlue-Badger/Zim-Rides.git
   ```

2. **Launch in Browser:**

   - **Option A: Direct File Open**
     Simply double-click `index.html` or drag it into your preferred web browser.

   - **Option B: Using Node.js Live Server**
     Run a lightweight local development server to support live reloading:
     ```bash
     npx live-server
     ```
     
