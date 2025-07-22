### ✅ `README.md` for Firebase Inventory Management App

````markdown
# 📦 Firebase Inventory Management App (Flutter)

This is a simple **Inventory Management System** built using **Flutter** and **Firebase Firestore**. It allows users to **Add**, **View**, **Update**, and **Delete** items in a real-time synced database — perfect for learning CRUD operations in a real-world mobile application.

---

## 📱 Features

- ✅ Add new inventory items with **Item Name, Category, Quantity, Price**
- 📋 View all items in a scrollable **ListView**
- ✏️ Update any item by tapping the edit icon
- 🗑️ Delete items in real-time
- 🔄 All data is synced live with **Firebase Firestore**
- ✅ Form field validation (e.g. price & quantity must be positive)
- ⚙️ Firebase configuration done using `flutterfire` CLI

---

## 🔥 Firebase Setup & Usage

- The app uses **Cloud Firestore** to store inventory data.
- Firebase is initialized via `firebase_core` and `cloud_firestore` Flutter packages.
- Configuration is done using the `flutterfire configure` CLI command which generates `firebase_options.dart`.

### 🔧 Firebase Collection Structure

The Firestore collection is named: `inventory`


---

## 💻 CRUD Operation Breakdown

### 🟢 Add Item

* Tap the **Add (+)** icon in the AppBar
* A form appears where user enters details
* On submit, data is sent to Firestore and list updates instantly

### 🔵 View Items

* Home screen displays all items in a scrollable list
* Each list item shows **Item Name**, **Category**, **Quantity**, **Price**

### 🟡 Update Item

* Tap the **edit icon** on any list item
* A pre-filled form opens
* Update details and save — Firestore is updated

### 🔴 Delete Item

* Tap the **delete icon** on any list item
* The item is removed from Firestore instantly

---

## 📁 File Structure

```
lib/
├── main.dart                # App Entry Point
├── firebase_options.dart    # Firebase config (auto-generated)
└── widgets/
    └── item_form.dart       # Reusable Add/Edit form widget
```

---

## ✅ Packages Used

| Package          | Purpose                   |
| ---------------- | ------------------------- |
| firebase\_core   | Initialize Firebase       |
| cloud\_firestore | Firestore database access |
| provider         | State management          |
| flutter          | UI toolkit                |

---

## 📽️ How This App Works

* The app starts at `main.dart`, which initializes Firebase using the auto-generated `firebase_options.dart`.
* The `MyHomePage` widget displays the real-time list from Firestore.
* Clicking the **Add** button shows the form using a modal dialog.
* Provider is used for managing the `TextEditingController` logic across widgets (optional).
* Any changes made are reflected in real-time using `StreamBuilder`.

---

## 🧪 Validation

* Quantity and Price must be **positive numbers**
* Item Name and Category are **required fields**

---

## 👨‍💻 Author

Syed Muhammad Usman
COMSATS University, 6th Semester
Flutter + Firebase Inventory App - Semester Project

---
