# 🌤️😄 Jokes & Weather 
A front-end application built with **TypeScript** and **Vite** that displays **random jokes**, **current weather**, and **sunrise/sunset times** using multiple external APIs. 
Styled with **pure CSS** and enhanced with simple animations for a fun and responsive user experience.



<div align="center">
  <img src="src/assets/ui-shoot/ui-shoot.png" width="75%" alt="Jokes & Weather App" />
</div>

[![Demo](https://img.shields.io/badge/View%20Demo-9932CC?style=for-the-badge)](https://jokes-and-weather.vercel.app/)

---

## 🚀 Features
- **Jokes API** — fetch random jokes with an interactive button. 
- **Rating system** — rate jokes using emojis (🤔, 🤭, 🤣). 
- **Weather API** — get live weather based on your location. 
- **SunTime API** — display sunrise and sunset times. 
- **UI/UX polish** — custom `@keyframes` animations.

---

## 🛠️ Technologies Used
- **Vite** — bundler and development server 
- **TypeScript** — logic and type safety 
- **CSS** — styling and animations 
- **External APIs**:
  - **ICanHazDadJoke** — https://icanhazdadjoke.com/ 
  - **Chuck Norris Jokes** — https://api.chucknorris.io/jokes/random 
  - **Nominatim** (OpenStreetMap) — geocoding (city → latitude/longitude) 
  - **Open-Meteo** — current weather data and sunrise and sunset times

---

## 🌐 API Details

### **1. ICanHazDadJoke**
Random general-purpose jokes.

**Endpoint**
GET https://icanhazdadjoke.com/


**Required header**
Accept: application/json


---

### **2. Chuck Norris Jokes API**
Random Chuck Norris–themed jokes.

**Endpoint**
GET https://api.chucknorris.io/jokes/random


---

### **3. Nominatim (OpenStreetMap)**
Converts a user’s city into latitude/longitude coordinates.

**Example**
https://nominatim.openstreetmap.org/search?q=${city}&format=json


---

### **4. Open-Meteo Weather API**
Provides current weather (temperature, wind speed, etc.).

**Endpoint used**
https://api.open-meteo.com/v1/forecast?latitude=${lat}&longitude=${lon}&current_weather=true


---

### **5. SunTime API**
Gets sunrise and sunset times based on coordinates.

**Endpoint used**
https://api.open-meteo.com/v1/forecast?latitude=${lat}&longitude=${lon}&daily=sunrise,sunset&timezone=auto



---

## 📂 Project Structure

```text
📂 S4-API/
├── 📄 index.html             # Root HTML file (entry point for Vite)
├── 📄 README.md              # Project documentation
├── 📄 package.json           # Dependencies and scripts
├── 📄 package-lock.json      # Dependency lock file
├── 📄 tsconfig.json          # TypeScript configuration
├── 📄 vite.config.js         # Vite configuration
├── 📄 eslint.config.js       # ESLint configuration
├── 📄 .gitignore             # Git ignore rules
├── 📂 public/                # Static assets
│   └── 🖼️ vite.svg           # Vite logo
├── 📂 node_modules/          # Installed dependencies
├── 📂 test/                  # Vitest testing files
│   ├── 🧪 jokeRanking.test.ts
│   └── 🧪 weatherApi.test.ts
└── 📂 src/
    ├── 📂 assets/            # Images and backgrounds
    ├── 📂 api/               # API modules
    ├── 📂 logic/             # Business logic
    │   ├── 📜 jokeRanking.ts
    │   ├── 📜 weatherdisplay.ts
    │   └── 📜 geolocation.ts
    ├── 📂 utils/             # Utility helpers
    │   └── 📜 weather-icons.ts
    ├── 📜 main.ts            # Application entry point
    └── 🎨 styles.css         # Global styles
\`\`\`

---

## ⚙️ Installation

Clone the repository and install the dependencies:

\`\`\`bash
git clone https://github.com/triflip/jokes-and-weather.git
cd jokes-and-weather
npm install
npm run dev
\`\`\`

---

## 🧪 Testing

The app uses **Vitest** to validate:

- API modules (`weatherApi`, `sunTimeApi`)
- Joke rating logic (`jokeRating`)
- Utility functions and UI components

Run the tests with:

\`\`\`bash
npx vitest
\`\`\`

---

## 📱 Responsive Design

The application is designed to provide a responsive experience across different screen sizes.

---

## 🎯 Project Goals

This project was built to practice:

- Working with multiple external APIs
- Managing asynchronous requests
- Handling API responses and errors
- Working with geolocation and coordinates
- Integrating TypeScript into a Vite project
- Organizing application logic into reusable modules
- Creating interactive UI elements with CSS animations
- Writing tests with Vitest

---

## 📚 What I Learned

Through this project, I strengthened my understanding of:

- TypeScript and type safety
- API integration
- Asynchronous JavaScript
- Data transformation
- Geolocation and external services
- Front-end testing with Vitest
- Separating API logic from UI logic
- Building responsive user interfaces

---

## 👤 Author

**Toni Valls**

[GitHub](https://github.com/triflip)
