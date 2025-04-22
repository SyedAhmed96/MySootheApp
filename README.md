# 🚀 Jetpack Compose Learning Series

Welcome to my Jetpack Compose Learning Series! This project is a hands-on exploration of the **Compose Essentials** and **Basic Layouts** in Jetpack Compose.

## 📘 What I’m Learning

This app is built with the goal of understanding the fundamental building blocks of Jetpack Compose—Android’s modern toolkit for building native UI. Here's a breakdown of the core concepts covered so far:

---

## 🧱 Composable Functions

At the heart of Jetpack Compose are **Composable functions**—the basic units of UI construction. A function annotated with `@Composable` tells the Compose compiler that this function is used to declare UI.

```kotlin
@Composable
fun Greeting(name: String) {
    Text(text = "Hello, $name!")
}
```

---

## 🎨 Surface

`Surface` is a composable that provides a Material Design background, elevation, shape, and other styling. It’s useful for wrapping your UI in a visually distinct container.

```kotlin
Surface(
    color = MaterialTheme.colorScheme.primary,
    modifier = Modifier.padding(16.dp)
) {
    Text(text = "Inside a Surface")
}
```

---

## 🧰 Modifier & Modifier Chaining

Modifiers allow you to **decorate or enhance** composables—apply padding, size, alignment, clickable behavior, and more. Chaining lets you stack multiple modifications in a readable way:

```kotlin
Text(
    text = "Chained Modifier Example",
    modifier = Modifier
        .padding(16.dp)
        .fillMaxWidth()
        .background(Color.Gray)
)
```

---

## 📐 Row and Column

Compose uses `Row` and `Column` to lay out elements **horizontally** and **vertically**, respectively. These are the Compose equivalents of LinearLayouts.

```kotlin
Row(
    modifier = Modifier.fillMaxWidth(),
    horizontalArrangement = Arrangement.SpaceBetween
) {
    Text("Left")
    Text("Right")
}

Column(
    modifier = Modifier.padding(16.dp),
    verticalArrangement = Arrangement.spacedBy(8.dp)
) {
    Text("Item 1")
    Text("Item 2")
}
```

---

## 🏷️ Resource Annotations

To fetch and display resources like strings or drawables, Compose provides helpful annotations and functions:

```kotlin
val label = stringResource(id = R.string.my_label)
val image = painterResource(id = R.drawable.my_image)

Text(text = label)
Image(painter = image, contentDescription = null)
```

---

## 💡 What's Inside?

- 🧱 `@Composable` functions with UI logic  
- 🎨 `Surface` usage for structured visual elements  
- 🔗 `Modifier` chaining for styling and layout  
- 📐 Basic layouts using `Row` and `Column`  
- 🖼️ Resource management using `stringResource` and `painterResource`  
- ✅ Clean and readable UI architecture  

---

## 🛠️ Tech Stack

- Kotlin  
- Jetpack Compose  
- Material 3 (optional depending on setup)  
- Android Studio Giraffe/Hedgehog or newer  

---

## 📦 Project Structure

```
📁 compose-learning-series
 ┣ 📁 ui
 ┃ ┣ 📄 MainScreen.kt
 ┃ ┗ 📄 Components.kt
 ┣ 📁 res
 ┃ ┣ 📄 strings.xml
 ┃ ┗ 📄 drawable/
 ┗ 📄 MainActivity.kt
```

---

## 🎯 Goal

This project is the foundation for more complex topics like:
- Theming
- Navigation
- State management
- Animations
- Custom layouts

---

## 📸 Screenshots

*(Coming Soon!)*

---

## 📚 References

- [Jetpack Compose Pathway](https://developer.android.com/jetpack/compose/tutorial)
- [Official Compose Docs](https://developer.android.com/jetpack/compose/documentation)
- [Material 3 Compose](https://developer.android.com/jetpack/compose/themes/material3)

---

Happy composing! 🎉
