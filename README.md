# 🍛 Tabarok-Go: Real-Time Community Food Tracker

**Tabarok-Go** is a lightweight, crowdsourced web application designed to help community members find and share information about "Tabarok" (community meals) at local mosques in real-time. Built specifically for the **Chandpur** region, it features live GPS tracking, auto-expiring data, and a dynamic mosque directory.

![License](https://img.shields.io/badge/license-MIT-green)
![Leaflet](https://img.shields.io/badge/Maps-Leaflet.js-orange)
![Database](https://img.shields.io/badge/Backend-SheetDB-red)

---

## ✨ Key Features

* **📍 Live Interactive Map:** Powered by Leaflet.js and OpenStreetMap.
* **🛰️ Find Near Me:** One-tap GPS localization to find the closest active Tabarak.
* **⏳ Auto-Expiration:** Entries automatically vanish after **2 hours** to ensure data freshness.
* **🏠 Address Memory:** Automatically suggests the last known address for a mosque to save users' time.
* **➕ Crowdsourced Locations:** Users can add new mosques by tapping directly on the map.
* **⚠️ Manual Close:** Ability to mark a meal as "Finished" to clear the map pin instantly.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
* **Maps API:** [Leaflet.js](https://leafletjs.com/)
* **Database/API:** [SheetDB](https://sheetdb.io/) (Google Sheets as a RESTful API)

---

## 🚀 Getting Started

### 1. Database Setup
1. Create a Google Sheet with two tabs:
   * **Tab 1 (`Sheet1`):** Headers: `id`, `Mosque`, `Food`, `Time`, `Address`, `Timestamp`.
   * **Tab 2 (`Mosques`):** Headers: `name`, `lat`, `lng`.
2. Connect your Google Sheet to [SheetDB](https://sheetdb.io/) to get your API URL.

### 2. Configuration
Open `index.html` and replace the `API` constant with your unique URL:
```javascript
const API = "[https://sheetdb.io/api/v1/your_id_here](https://sheetdb.io/api/v1/your_id_here)";
```
# 3. Deployment
​Simply upload the index.html file to GitHub Pages, Netlify, or Vercel.
​# 📱 User Guide
​Finding Food: Active Tabarok locations are marked with a Bell Icon. Tap the pin to see the menu, time, and address.
​Updating Info: Tap a blue pin, enter the food and time, and hit Save. The pin will turn into a bell for all users.
​Adding a Mosque: Click "Add New Mosque," tap the exact spot on the map, provide a name, and submit.
​GPS Search: Click "Find Near Me" to see where you are and get directed to the nearest meal.
​# 🤝 Contributing
​Contributions are welcome! If you have ideas for features (like WhatsApp sharing or countdown timers), feel free to fork the repo and submit a pull request.
# ​🛡️ License
​Distributed under the MIT License. See LICENSE for more information.
​Developed with ❤️ by Aftab Sunny |
