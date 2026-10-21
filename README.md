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

Button btnSecondActivity = findViewById(R.id.btnSecondActivity);

### 2. Handling the Click Event (`setOnClickListener`)
An `OnClickListener` detects when the user presses the button and triggers the transition:

btnSecondActivity.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {
        Intent intent = new Intent(MainActivity.this, SecondActivity.class);
        startActivity(intent);
    }
});

### 3. Explicit Intent & Navigation
An Explicit Intent specifies the exact destination component (`SecondActivity.class`). Calling `startActivity(intent)` tells the Android OS to launch `SecondActivity` and push it onto the Activity back stack.

## 🚀 How to Run
1. Clone or download this repository.
2. Open the project folder in **Android Studio**.
3. Allow Gradle to sync dependencies.
4. Run on an Android emulator or physical device (`Shift + F10`).
