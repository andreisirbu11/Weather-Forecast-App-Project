# 🌤️ Weather Forecast App

This is a simple weather forecast web app built with **Node.js**, **Express**, **Axios**, and **EJS**. The app fetches weather data from the [7Timer! API](http://www.7timer.info/doc.php) based on the user's provided latitude and longitude, and presents current and upcoming weather conditions with descriptive icons.

## 📌 Features

- Automatically detects user's current location using the browser's geolocation API (with user permission).
- Displays today's weather with relevant icon and temperature.
- Shows 6-day forecast with icons, daily highs and lows.
- Responsive UI styled using **Bootstrap**.
- Fully dynamic using **EJS** templating.
- Icons represent conditions like clear, rain, cloudy, fog, snow, etc.

## 🛠️ Tech Stack

- **Backend:** Node.js, Express
- **Frontend:** HTML, CSS (Bootstrap), JavaScript
- **Templating Engine:** EJS
- **HTTP Client:** Axios
- **API:** [7Timer!](http://www.7timer.info/)

## 🗂️ Project Structure

```
/public
├── /assets/*.svg           # Weather icons (SVG)
├── /style/style.css        # Custom CSS styles
└── /script/script.js       # Client-side JS
/views
└── index.ejs               # Main UI rendered by server
index.js                    # Express server logic
package.json                # Project dependencies
```


## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/en/download/) installed

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/weather-app.git
    cd weather-app

2. Install dependencies:
    ```bash
    npm install

3. Start the server:
    ```bash
    node index.js

4. Open your browser and visit:
    ```bash
    http://localhost:3000

## 🔄 API Integration
This project uses the 7Timer! API which returns weather data in JSON format. The server sends a request using Axios and passes the data to the EJS frontend for rendering.

## 🐛 Error Handling
- Server logs error messages when API calls fail.
- User is shown a fallback message if weather data is unavailable.

## 📄 License
This project is open source and available under the [MIT License](LICENSE).