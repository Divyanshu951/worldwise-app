# 🌍 WorldWise

**WorldWise** is a React single-page application that lets you track your travels around the world on an interactive map.

---

## ✨ Features

### 🗺️ Interactive Map

- Explore the world using a fully interactive **Leaflet** map.
- Click anywhere on the map to add a new city to your travel log.
- Navigate to any saved city by clicking on it in the sidebar.

### 🏙️ City Management

- **Add cities** — Log a visited city with notes, date, and auto-detected country/emoji.
- **View city details** — See detailed information about each tracked city.
- **Delete cities** — Remove cities you no longer want in your list.
- Cities and countries are synced with a **remote REST API** (MockAPI).

### 🌐 Country List

- Automatically groups your visited cities by country.
- Displays country flags using native emoji support.

### 🔐 Fake Authentication

- Protected routes with a simulated login/logout flow.
- Only authenticated users can access the main app and map.

### ⚡ Performance Optimizations

- **Code splitting** with `React.lazy()` and `Suspense` for faster initial page loads.
- **Memoization** with `useCallback` to prevent unnecessary re-renders.

### 📍 Geolocation

- Detect the user's current position via the browser **Geolocation API**.
- Quickly navigate the map to your current location.

---

## 🛠️ Tech Stack

| Technology                   | Purpose                             |
| ---------------------------- | ----------------------------------- |
| **React 18**                 | UI library                          |
| **React Router 6**           | Client-side routing & nested routes |
| **Context API + useReducer** | Global state management             |
| **Leaflet / React-Leaflet**  | Interactive map rendering           |
| **React DatePicker**         | Date selection for city entries     |
| **CSS Modules**              | Component-scoped styling            |
| **Vite**                     | Dev server & build tool             |
| **MockAPI**                  | Remote REST API for city data       |

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v16+)
- **npm**

### Installation

```bash
# Clone the repo
git clone https://github.com/<your-username>/worldwise.git
cd worldwise

# Install dependencies
npm install

# Start the dev server
npm run dev
```

The app will be available at `http://localhost:5173`.

---

## 📁 Project Structure

```
src/
├── components/       # Reusable UI components (Map, CityList, Form, etc.)
├── contexts/         # React Context providers (Cities, Auth)
├── hooks/            # Custom hooks (useGeolocation, useUrlPosition)
├── pages/            # Route-level page components
├── App.jsx           # Root component with routing
├── main.jsx          # Entry point
└── index.css         # Global styles
```

---

This project was built as part of [Jonas Schmedtmann's Ultimate React Course](https://www.udemy.com/course/the-ultimate-react-course/) to practice advanced React patterns and real-world application architecture.
