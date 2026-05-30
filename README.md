
# Community Core Stack — Damped Springs

> A simple yet powerful package to instantly improve your game feel using modern, physics-based Damped Springs.

---

## What is this?

A minimalist implementation of Damped Springs inspired by the classic video: *Instant "Game Feel" Tutorial - Secrets of Springs Explained*.

Since this math is public knowledge, I decided to make it accessible to all Unity Developers. This package warps the spring math into incredibly easy-to-use **Extension Methods**, allowing you to choose between continuous `Update` execution or modern `async/await` single-line animations using Unity's **Awaitable API**.

---

## 🚀 Quick Start (Single Line Magic)

Forget complex setup ceremonies. You can animate anything in a single line of code without cluttering your scripts with update loops or velocity variables:

```csharp
using FGT.Tools.Springify;
using UnityEngine;

// 1. Move a Transform to a target position
_affectedObject.SpringToAsync(_target.position, frequency: 5f, damping: 0.5f);

// 2. Animate a UI Slider value smoothly
_slider.value.SpringToAsync(targetValue, val => _slider.value = val, frequency: 2f, damping: 0.25f, this, "slider");

// 3. Change Camera FOV elastically (Immune to button spamming)
_camera.fieldOfView.SpringToAsync(targetFOV, fov => _camera.fieldOfView = fov, frequency: 5f, damping: 0.5f, this, "cam_fov");
```

---

## ⚙️ How to Install (Unity Package Manager)

You can install this package directly via the Unity Package Manager using the Git URL:

1. Open `Window` -> `Package Manager` in Unity.
2. Click the `+` button in the top-left corner.
3. Select `Add package from git URL...`.
4. Paste the following URL: `https://github.com/lucspinto/com.ponderado.springtween.git` *(Ajuste com a URL real do seu repositório)*

---

## 📦 Looking for Production-Ready Samples?

While the core source code is 100% free here on GitHub, a premium version **(Springify)** featuring **fully set up interactive demo scenes** (including UI Sliders, interactive Rotation Wheels, Juice Scale popping, and Camera FOV transitions) is available on the **Unity Asset Store.**

Buying the Asset Store version is the best way to support this open-source initiative and save hours of production setup!

---

## 📄 License

**CC0 - No Rights Reserved.**

This is part of the Community Core Stack initiative.
No credit is required, though it's always appreciated!

---

## What is Community Core Stack?

Game development moves faster when the community builds together. **Community Core Stack** is an open initiative to produce high-quality, ready-to-use, lightweight utilities that anyone can pick up, learn from, and build upon.

Everyone can contribute.

---

## Author

Made with ☕ by **lucspinto** Part of the *Game Dev Creative* series — focused on the visual, creative, and juicy side of Unity game development.

* **LinkedIn:** [linkedin.com/in/lucspinto](https://www.linkedin.com/in/lucspinto)
* **GitHub:** [github.com/lucspinto](https://github.com/lucspinto)
* **Website:** [Ponderado Game Dev](https://web-ponderado-game-dev.vercel.app/)
* **Courses:** [Udemy Courses](https://www.udemy.com/user/lucas-r-pinto/)
