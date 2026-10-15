# Simple Gemini AI Chatbot (Android)

A lightweight, clean Android AI Chatbot built using Kotlin, RecyclerView, and the Google Gen AI SDK (Gemini API).

## 📱 App Preview
Here is how the clean WhatsApp-style UI looks in action:

> *(You can add your app screenshot image named `screenshot.png` to this folder to display it here)*

```
 +----------------------------------+
 |  [User: hi]                      |
 |  [AI: Hello! How can I help...]  |
 |                                  |
 |  [User: what is ai]              |
 |  [AI: **AI** stands for...]      |
 +----------------------------------+
 | Message...               [Send]  |
 +----------------------------------+
```

## Features
- **WhatsApp-style UI:** User messages on the right (green bubble) and AI responses on the left (gray bubble).
- **RecyclerView Adapter:** Optimized and written with simple, clean identifiers.
- **Gemini Powered:** Uses `gemini-1.5-flash` for fast and intelligent text generation.

## Setup Instructions
1. Add the Internet permission in your `AndroidManifest.xml`:
   ```xml
   <uses-permission android:name="android.permission.INTERNET" />
   ```
2. Add the dependencies in your `app/build.gradle.kts`:
   ```kotlin
   implementation("com.google.ai.client.generativeai:generativeai:0.9.0")
   implementation("org.jetbrains.kotlinx:kotlinx-coroutines-android:1.7.3")
   ```
3. Add your Google Gemini API key in `AiChatBot.kt`:
   ```kotlin
   val g = GenerativeModel(
       modelName = "gemini-1.5-flash",
       apiKey = "YOUR_API_KEY"
   )
   ```
