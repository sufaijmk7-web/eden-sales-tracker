# Eden Sales Tracker (Realtime Firebase Version)

This is a live sales, staff, and inventory tracking system for Eden Perfume. It uses **Firebase Realtime Database** to sync data instantly across multiple devices and locations.

## 🌐 Live Features

- 📦 Track and manage product inventory
- 👥 Manage employees and their attendance
- 💰 Log and monitor sales transactions
- 🏬 Handle multiple store locations
- 🔁 All updates sync in real-time using Firebase

## 🔧 Technologies Used

- HTML, CSS, JavaScript (Vanilla)
- Firebase Realtime Database
- Firebase Hosting (optional for deployment)

## 🚀 How It Works

1. Data is stored in Firebase Realtime Database at:
   ```
   https://eden-sales-2025-default-rtdb.asia-southeast1.firebasedatabase.app/
   ```
2. JavaScript connects to Firebase and listens for changes using `onValue()`.
3. UI updates live for:
   - Employees (`/employees`)
   - Products (`/products`)
   - Sales (`/sales`)
   - Stores (`/stores`)
   - Attendance (`/attendance`)

## 📁 Firebase Data Structure

```json
{
  "employees": {
    "admin": {
      "username": "admin",
      "password": "1234",
      "store": "Main",
      "role": "manager"
    }
  },
  "products": {
    "1": {
      "product": "Rose Perfume",
      "price": 49.99,
      "quantity": 100,
      "store": "Main"
    }
  },
  "sales": {
    "1": {
      "product": "Rose Perfume",
      "quantity": 2,
      "date": "2025-08-02",
      "employee": "admin",
      "store": "Main"
    }
  },
  "stores": {
    "1": {
      "store": "Main"
    }
  },
  "attendance": {
    "1": {
      "username": "admin",
      "date": "2025-08-02",
      "checkIn": "09:00",
      "checkOut": "17:00"
    }
  }
}
```

## 🧪 Local Testing

1. Open `index_with_rendering.html` in a browser.
2. Data is pulled live from Firebase.
3. Try editing your Firebase DB — the UI updates instantly.

## 📦 Future Improvements

- User login/authentication
- Editable forms and delete buttons
- Mobile-friendly UI

## 📄 License

MIT License (or your preferred license)
