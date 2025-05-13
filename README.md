# food-application

A beginner-friendly **Food Ordering App** built with **Jetpack Compose** and **Material 3**. The app allows users to log in using just their name, view a list of food items with prices and images, and place orders that display confirmation messages.

---

## 🔥 Features

- 🔐 Simple login screen (no password needed)
- 🍕 Food items with name, image, description, and price
- 🛒 "Order Now" functionality with a Snackbar confirmation
- 🎨 Material Design 3 UI
- ⚙️ Modern Android development with **Jetpack Compose**
- 📦 Clean architecture with composable UI

---

## 🛠️ Tech Stack

- **Language:** Kotlin
- **UI Toolkit:** Jetpack Compose
- **Theme:** Material 3 (Material You)
- **Architecture:** Declarative UI, Composable Functions
- **State Management:** `remember`, `mutableStateOf`

---

## 📁 Project Structure

```

com.example.foodapp/
├── MainActivity.kt             # App entry point and navigation logic
├── AppContent()                # Controls login vs. food list UI
├── LoginScreen()               # Login screen UI
├── FoodListScreen()           # Food listing screen
├── TopBar()                    # App bar with user greeting
├── FoodCard()                  # UI card for each food item
├── FoodItem.kt                 # Data class for food items
└── res/drawable/               # Images for burger, pizza, pasta

````

---

## ⚙️ How to Run Locally

### ✅ Prerequisites

- Android Studio (Arctic Fox or later)
- Kotlin 1.8+
- Android SDK 31+

### 🧩 Gradle Setup

Ensure your `build.gradle (Module)` has the following dependencies:

```gradle
dependencies {
    implementation "androidx.core:core-ktx:1.12.0"
    implementation "androidx.activity:activity-compose:1.9.0"
    implementation "androidx.compose.material3:material3:1.2.0"
    implementation "androidx.lifecycle:lifecycle-runtime-ktx:2.7.0"
    implementation "androidx.compose.ui:ui-tooling-preview:1.5.0"
    implementation "androidx.compose.foundation:foundation:1.5.0"
}
````

In your `build.gradle (Project)` file:

```gradle
buildscript {
    ext {
        compose_ui_version = '1.5.0'
    }
}
```

Make sure `Jetpack Compose` is enabled in your `android` block:

```gradle
buildFeatures {
    compose true
}
composeOptions {
    kotlinCompilerExtensionVersion = "1.5.0"
}
```

---

## 🎨 Assets Required

Place these images in `res/drawable/`:

* `burger.png` or `burger.jpg`
* `pizza.png` or `pizza.jpg`
* `pasta.png` or `pasta.jpg`

You can download free assets from [https://www.flaticon.com/](https://www.flaticon.com/) or similar royalty-free image sites.

---

## 📝 Future Enhancements

* 🛍 Add cart & checkout system
* 🔐 Implement user authentication (Firebase)
* 💳 Integrate payment gateway
* 🌐 Connect to a backend/database
* 📱 Add ViewModel & Navigation Component

---

