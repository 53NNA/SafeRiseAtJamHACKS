# SafeRise 🌊 — Flood Risk Visualizer & Evacuation Advisor

SafeRise is an interactive web tool designed to help users assess flood risks at any location around the world. By combining elevation data, rainfall simulation, and evacuation pathfinding, SafeRise provides real-time insights to support disaster preparedness and decision-making.

🚀 Built for **JamHacks 9**

---

## 🌍 Features
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/blob/main/original-2.png)
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/raw/main/original-3.png)
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/raw/main/original-4.png)
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/raw/main/original-6.png)
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/raw/main/original-8.png)
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/raw/main/original-9.png)
![Alt text](https://github.com/53NNA/SafeRiseAtJamHACKS/raw/main/original-10.png)

---

## 🧠 How It Works

1. **User clicks on a location**  
   ↳ We fetch elevation via our backend `/elevation` endpoint.

2. **Flood simulation is generated**  
   ↳ Based on selected rainfall and terrain data, a predicted flood height is calculated.

3. **Safety advice is provided**  
   ↳ Depending on elevation, users are warned or routed to nearby safe zones.

4. **Routing API kicks in (if needed)**  
   ↳ Using OpenRouteService, the shortest driving path to safety is displayed.

---

## 🔧 Tech Stack

- **Frontend**: HTML, CSS, JavaScript, Leaflet.js
- **APIs**:
  - 🌦️ OpenWeatherMap (planned for historical rainfall data)
  - 🌍 Mapbox (map tiles)
  - 🗺️ OpenRouteService (routing)
  - 🧭 Nominatim (reverse geocoding)
  - 📡 Custom Elevation API (using Google or Open-Elevation backend)

---

## 📦 Getting Started

```bash
# Clone the repo
git clone https://github.com/your-username/saferise.git
cd saferise

# Serve the app (using any local server, e.g. Python or Live Server)
python3 -m http.server
