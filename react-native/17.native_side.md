# 📱 Native Side in React Native

---

#  Learning Objectives

After completing this module, you will be able to:

- Understand Native Modules
- Understand Native UI Components
- Learn how the Bridge works
- Understand JSI
- Learn Turbo Modules
- Understand Fabric
- Know when native code is required

---

# 1️⃣ What is the Native Side?

React Native apps contain two worlds:

- JavaScript (React Native)
- Native Platform (Android & iOS)

Native code is written in:

- Android → Kotlin / Java
- iOS → Swift / Objective-C

---

# 2️⃣ React Native Architecture

```text
React Native App
        │
 JavaScript Code
        │
React Native Runtime
        │
Native Android / iOS APIs
        │
Camera • GPS • Bluetooth • Files
```

---

# 3️⃣ Native Modules

Native Modules expose platform-specific functionality to JavaScript.

Examples:

- Camera
- Bluetooth
- NFC
- Biometrics
- Battery
- Sensors

### Why Use Native Modules?

Sometimes JavaScript alone cannot access all device capabilities.

---

# 4️⃣ Native UI Components

Native UI Components wrap platform-specific views.

Examples:

- Google Maps
- Video Player
- Camera Preview
- Native Charts

They allow React Native apps to use real native controls.

---

# 5️⃣ The Bridge (Old Architecture)

The Bridge transfers messages between JavaScript and native code.

```text
JavaScript
     │
   Bridge
     │
Native Code
```

### Limitations

- Asynchronous communication
- Serialization overhead
- Performance bottlenecks for heavy workloads

---

# 6️⃣ JSI (JavaScript Interface)

JSI allows JavaScript to communicate directly with native code.

```text
JavaScript
     │
    JSI
     │
Native Code
```

### Benefits

- Faster execution
- Less overhead
- Better performance
- Foundation of the New Architecture

---

# 7️⃣ Turbo Modules

Turbo Modules replace the old Native Module system.

### Advantages

- Lazy loading
- Faster startup
- Better memory usage
- Direct JSI communication

Use Turbo Modules when building modern native integrations.

---

# 8️⃣ Fabric

Fabric is React Native's new rendering system.

### Benefits

- Faster UI updates
- Better concurrency
- Improved rendering performance
- Better integration with React

---

# 9️⃣ Old vs New Architecture

| Feature | Old Architecture | New Architecture |
|---------|------------------|------------------|
| Communication | Bridge | JSI |
| Native Modules | Classic | Turbo Modules |
| UI Renderer | Legacy | Fabric |
| Performance | Good | Better |
| Startup | Slower | Faster |

---

# 🔟 When Do You Need Native Code?

Use native development when:

- Custom hardware integration
- Bluetooth/NFC
- Advanced camera features
- Custom SDKs
- Payment terminals
- Enterprise device APIs

Most Expo applications do **not** require writing native code.

---

#  Best Practices

- Prefer Expo libraries when available.
- Use native modules only when necessary.
- Keep JavaScript and native logic separated.
- Upgrade to the New Architecture for better performance.

---

#  Common Mistakes

- Assuming every feature needs native code
- Overusing custom native modules
- Ignoring platform differences
- Mixing business logic with native code

---

# 💼 Interview Questions

1. What are Native Modules?
2. What are Native UI Components?
3. What is the React Native Bridge?
4. Why was JSI introduced?
5. What are Turbo Modules?
6. What is Fabric?
7. Bridge vs JSI?
8. Old vs New Architecture?
9. When should you write native code?
10. Why is the New Architecture faster?

---

#  Mini Project

Design the architecture for a React Native app that uses:

- Camera
- GPS
- Bluetooth
- Push Notifications
- Payment SDK

Identify which parts use JavaScript and which rely on native APIs.

---

#  Key Takeaways

- React Native combines JavaScript with native Android and iOS code.
- Native Modules expose platform features.
- Native UI Components render real native views.
- The Bridge was used in the old architecture.
- JSI enables direct communication.
- Turbo Modules and Fabric are key parts of the New React Native Architecture.


