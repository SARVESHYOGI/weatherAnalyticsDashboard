# 🌤️ Weather Analytics Dashboard

A modern, responsive **Weather Analytics Dashboard** built with **React**, **TypeScript**, **Redux Toolkit**, **Firebase Authentication**, and **Recharts**.  
It provides real-time weather insights, multi-city tracking, favorites, and detailed analytics with a clean UI.

---

## 🚀 Live Features

### 🔐 Authentication
- Google Sign-In using Firebase
- Secure protected routes
- Persistent login state

### 🏙️ Multi-City Dashboard
- Track multiple cities at once
- Real-time updates (data refreshed every 60s)
- Cached responses to reduce API calls
- Clean summary cards for each city including:
  - Temperature
  - Condition icon
  - Humidity
  - Wind speed
  - Last updated time

### ⭐ Favorites
- Add / remove favorite cities
- Favorites persist per user
- Dedicated favorites page

### 📊 Analytics & Charts
- Hourly temperature line chart
- 7-day temperature bar chart
- Responsive & interactive charts (Recharts)
- Smooth UX on desktop & mobile

### 🔍 City Search
- Debounced city search
- Add cities dynamically to dashboard
- Prevents duplicates automatically

### ⚙️ Settings
- Unit toggle (°C / °F)
- Instant UI updates without refetching
- Global state powered by Redux

### 📱 Responsive UI
- Mobile-friendly layout
- Grid adapts to screen size
- Smooth hover & transition effects

### 🧠 Advanced Features (Bonus Points)
- ✔ Google Authentication
- ✔ Real-time data fetching
- ✔ Data freshness < 60 seconds
- ✔ API caching layer
- ✔ Redux global state management
- ✔ Typed hooks (TypeScript best practices)
- ✔ Clean architecture

---

## 🛠️ Tech Stack

**Frontend**
- React + TypeScript
- Vite
- Tailwind CSS
- React Router
- Redux Toolkit
- Recharts

**Backend / Services**
- WeatherAPI.com
- Firebase Authentication

---

## 📁 Project Structure
```
src/
│
├── app/ # Redux store setup
├── components/ # UI components
│ ├── Auth/
│ ├── Dashboard/
│ ├── Charts/
│ ├── Common/
│ └── Layout/
│
├── features/ # Redux slices
│ ├── auth/
│ ├── weather/
│ ├── favorites/
│ └── settings/
│
├── hooks/ # Custom hooks
├── pages/ # Route pages
├── utils/ # Helpers & formatters
├── firebase.ts # Firebase config
└── main.tsx
```

---

## ⚙️ Environment Variables

Create a `.env` file in the root directory:

```env
VITE_WEATHER_API_KEY=your_weatherapi_key

VITE_FIREBASE_API_KEY=your_firebase_key
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_APP_ID=your_app_id

```

## ▶️ Run Locally
### Install dependencies

`npm install`

### Start dev server
`npm run dev`

## 🧩 Architecture Highlights

Redux Toolkit for predictable state management

Caching layer to avoid unnecessary API calls

Derived UI state (no duplicated local state)

Typed hooks (useAppDispatch, useAppSelector)

Separation of concerns (features, components, hooks)

Reusable chart components

Pure functions & clean effects
