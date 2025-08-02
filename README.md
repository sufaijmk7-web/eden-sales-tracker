# Eden Sales Tracker (Live Realtime Firebase App)

A web-based sales and inventory management platform for Eden Perfume, powered by **Firebase Realtime Database**.

## 📦 Features

- 👥 Staff management
- 🧴 Product inventory tracking
- 💰 Live sales logging
- 🕒 Attendance recording
- 🏬 Multi-store support
- 🔁 Real-time sync across all devices and locations

## 🔧 Built With

- HTML, CSS, JavaScript (vanilla)
- Firebase Realtime Database
- Firebase Hosting

## 📂 Firebase Structure

The following collections are used inside Realtime Database:

```
/employees
/products
/sales
/stores
/attendance
```

Each holds nested data like:

```json
"employees": {
  "admin": {
    "username": "admin",
    "password": "1234",
    "store": "Main",
    "role": "manager"
  }
}
```

## 🚀 Deployment (Firebase Hosting)

To deploy the app online:

1. Install Firebase CLI:
   ```bash
   npm install -g firebase-tools
   ```

2. Log in:
   ```bash
   firebase login
   ```

3. Initialize:
   ```bash
   firebase init
   ```

4. Deploy:
   ```bash
   firebase deploy
   ```

Live version will be hosted at:
```
https://eden-sales-2025.web.app
```

> Make sure your `index.html` connects to your Firebase Realtime DB at:
> `https://eden-sales-2025-default-rtdb.asia-southeast1.firebasedatabase.app/`

## 📄 License

MIT (or update to your preferred license)
