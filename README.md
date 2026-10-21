# Android Activities & Intents Assignment

A simple Android application created to practice Activity lifecycles, Button click events, and navigating between screens using Explicit Intents.

---

## 📱 Features & Workflow
- **MainActivity:** Displays the main screen with a button labeled **"Second Activity"**.
- **Button Click Handling:** Listens for user tap events using `View.OnClickListener`.
- **Screen Navigation:** Uses an **Explicit Intent** to transition from `MainActivity` to `SecondActivity`.
- **SecondActivity:** Displays a welcoming message: *"Welcome to Second Activity!"*.

---

## 🛠️ Built With
- **IDE:** Android Studio
- **Language:** Java
- **UI:** XML (ConstraintLayout)
- **Target SDK:** Android API 34+

---

## 💡 How It Works

### 1. Linking the Button (`findViewById`)
The button defined in the XML layout (`activity_main.xml`) is referenced in Java:
```java
Button btnSecondActivity = findViewById(R.id.btnSecondActivity);
