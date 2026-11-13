# 🍲 TYFOOD at HOME - Hyperlocal Food Ordering Platform

A food ordering and delivery ecosystem connecting **Clients**, **Restaurants**, and **Delivery Partners** in real-time.

---

## 🌟 The 3 Connected Sides

### 1️⃣ Client (Customer) Portal (`index.html`)
- **Visual Food Discovery:** Browse restaurants and dishes with appetizing 4K culinary photography.
- **Dietary Filter:** Instant filtering for Veg, Non-Veg, Burgers, Pizzas, Biryani, Curries, and Desserts.
- **Cart & Seamless Checkout:** Live subtotal, 5% taxes, dynamic delivery calculation, and custom cooking instructions.
- **Live Order Tracking:**
  - Real-time step progress (Placed ➔ Accepted ➔ Cooking ➔ Ready ➔ Out for Delivery ➔ Delivered).
  - **Restaurant Food Making Time Countdown:** Live ticking timer (`MM:SS`) set by the chef in the kitchen.
  - **Live GPS Map Tracking (Leaflet & OpenStreetMap):** Moving delivery rider marker along city streets with speed, distance, and ETA metrics.
  - **Verified Rider Profile:** Displays assigned partner, vehicle plate, verified driving license check, and rating.

---

### 2️⃣ Restaurant (Kitchen) Portal (`restaurant.html`)
- **Kitchen Order Pipeline:** Real-time incoming order alert with bell chimes.
- **Food Making Time Manager:** Select or customize preparation duration (e.g. 10m quick, 15m standard, 20m, 30m feast) with ticking kitchen display timers.
- **Handoff Alert:** "Mark Food Ready for Pickup" instantly notifies delivery partners on their radar.
- **High-Definition Dish Creator (New):**
  - Add new dishes with 4K food photography presets (Gourmet Burgers, Woodfired Pizza, Saffron Dum Biryani, Crispy Wings, Truffle Fries, etc.) or custom high-res URLs and device uploads.
  - Stock management: Toggle dishes in-stock or sold-out.
- **Restaurant Earnings & Financial Ledger (New):**
  - Gross sales counter, 10% platform commission deduction, and 90% net kitchen profit ledger.
  - Order-by-order transparent financial receipts.

---

### 3️⃣ Delivery Partner Fleet Portal (`delivery.html`)
- **Partner Sign-Up & Mandatory Driving License Check (New):**
  - Name, mobile, vehicle type (Scooter, Motorcycle, EV, Bicycle), and vehicle registration number.
  - Driving License validation check (strict regional format verification).
  - Driving License front document upload & photo card scanner viewer.
  - Verified Partner badge (`✓ Driving License Verified`).
- **Earnings Formula Strictly at ₹10 per Kilometer (New):**
  - Guaranteed rate: **`₹10 / KM`**.
  - Order payout breakdown: `Distance (e.g. 4.2 km) × ₹10/km = ₹42`.
  - Rider Wallet Dashboard: Total Balance, total kilometers driven, trips completed, and instant bank withdrawal simulator.
- **Live GPS Navigation Simulator:**
  - Real-time city street routing from Restaurant to Customer.
  - Auto-drive controls (1x real-time, 2x fast, 5x turbo speed) and manual step-by-step turns.
  - Street guidance prompts and speed HUD.
  - Order completion with instant wallet credit!

---

### ⚡ 4️⃣ Unified 3-in-1 Live Control Center (`split-view.html`)
- Displays all **3 portals side-by-side on one screen**.
- Watch in real-time as an order placed on the left side alerts the restaurant in the middle, and the delivery partner on the right accepts, auto-drives GPS, and delivers!
- Quick-flow trigger buttons to test the entire lifecycle in seconds.

---

## 🛠️ How All Three Connect
1. **BroadcastChannel API (`tyfood_event_bus`):** Instant sub-millisecond event streaming between browser tabs and frames.
2. **`localStorage` Synchronization:** Persistent state and cross-tab storage event listeners.
3. **Web Audio API Synthesizer:** Built-in acoustic feedback (kitchen chimes, motorcycle horn, order bell, celebration chords) with zero external audio dependencies.
4. **Leaflet.js & OpenStreetMap:** High-performance interactive GPS mapping and waypoint interpolation.

---

## 🔑 Login ID System & Credentials

Each portal provides dedicated **Login ID** management, quick demo account switchers, and new user registration:

| Role | Default Demo Login ID | Profile / Identity | Key Capability |
| :--- | :--- | :--- | :--- |
| **Client (Customer)** | `client.tanmay@tyfood.com`<br>`client.priya@tyfood.com` | Tanmay Yadav (Sector 18)<br>Priya Sharma (Palm Meadows) | Browse restaurants, place orders, real-time tracking with countdown timer & live Leaflet rider map. |
| **Restaurant (Kitchen)** | `chef.burgerloft@tyfood.com`<br>`chef.bellaitalia@tyfood.com`<br>`chef.royalbiryani@tyfood.com` | The Burger Loft & Grills<br>Bella Italia Pizzeria<br>Royal Biryani Kitchen | **Register new restaurant**, FSSAI verification, accept orders, set food making timers, **add dishes with 4K photos**, view 90% net earnings. |
| **Delivery Partner** | `rider.vikram@tyfood.com`<br>`rider.aman@tyfood.com` | Vikram Singh (Activa 6G)<br>Aman Sharma (Ather EV) | Driving license check & upload, accept jobs, live GPS navigation simulation, **earnings at ₹10/km**, wallet balance & payouts. |

---

## 🏪 Restaurant Sign-Up & Guided Dish Addition Flow
1. Open [`restaurant.html`](file:///c:/Users/Dell/OneDrive/Desktop/TYFOOD/restaurant.html) and click **"🏪 + Register New Restaurant"**.
2. Complete the onboarding form:
   - Restaurant Brand Name, Owner Name, Business Phone & Email.
   - **FSSAI License Number** (with active food safety validation check).
   - Kitchen Address, Cuisine Specialties, and Avg Prep Time.
   - High-Res Restaurant Ambiance Cover Photo Preset or custom URL.
   - Payout UPI ID / Bank Account for receiving daily 90% net earnings.
3. Upon registration:
   - Account is created with a unique Login ID (e.g. `chef.yourrestaurant@tyfood.com`).
   - Automatically opens the **"📸 + Add Dish to Menu"** modal!
   - Select 4K culinary food presets (Burgers, Pizza, Biryani, Wings, Pasta, Fries, Desserts) or paste a custom high-definition food image URL.
   - The newly added dishes become immediately available for ordering in the Client Portal!

---

## 🚀 How to Run the Website
Simply double-click any of the HTML files to open in your browser (Google Chrome, Microsoft Edge, Firefox, or Safari):

- Open `index.html` for the Customer Portal.
- Open `restaurant.html` for the Kitchen & Menu Management.
- Open `delivery.html` for the Delivery Partner Fleet & GPS Tracker.
- Open `split-view.html` to see all 3 connected together live side-by-side!

