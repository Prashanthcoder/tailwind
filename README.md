# 🍽️ AI Nutritionist

![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-active-success)
![Tech](https://img.shields.io/badge/stack-FastAPI%20%7C%20HTML%20%7C%20TailwindCSS-blue)

AI Nutritionist is a simple full‑stack web application that allows users to upload a food image and get an AI‑based prediction of what the food is, along with confidence information. It is designed as a clean, beginner‑friendly project that demonstrates frontend–backend integration with machine learning inference.

---

## 🚀 What the project does

* Provides a modern web UI to upload food images
* Sends images to a backend API for prediction
* Displays predicted food label and confidence score
* Shows image preview before upload
* Handles loading and error states gracefully

The frontend is built using **HTML + Tailwind CSS**, while the backend exposes a `/predict` API endpoint (implemented separately, typically using **FastAPI**).

---

## 💡 Why this project is useful

* Great learning reference for **full‑stack ML projects**
* Demonstrates **image upload handling** using `FormData`
* Shows clean **frontend–backend communication** via `fetch`
* Minimal and readable codebase, easy to extend
* Ideal starting point for projects like:

  * AI Nutrition Tracker
  * MyFitnessPal‑style apps
  * Food calorie estimation systems

---

## 🧩 Tech Stack

* **Frontend**: HTML, Tailwind CSS, Vanilla JavaScript
* **Backend**: FastAPI (hosted separately)
* **ML**: Image classification model (dummy or real, backend‑side)
* **Hosting**:

  * Frontend: Static hosting (GitHub Pages / Netlify)
  * Backend: Render

---

## ⚙️ How to get started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/ai-nutritionist.git
cd ai-nutritionist
```

### 2️⃣ Open the frontend

This project uses plain HTML, so you can directly open the file:

```bash
index.html
```

Or serve it using a local server (recommended):

```bash
python -m http.server 8000
```

Then open:

```
http://localhost:8000
```

### 3️⃣ Configure backend endpoint

In `index.html`, update the API URL if needed:

```js
fetch("https://tailwind1-ikqo.onrender.com/predict", {
  method: "POST",
  body: formData
});
```

Ensure the backend `/predict` endpoint:

* Accepts multipart file uploads
* Returns JSON with:

  * `prediction`
  * `confidence`
  * `filename`
  * `size_kb`

---

## 🧪 Example API Response

```json
{
  "message": "Prediction successful",
  "prediction": "Pizza",
  "confidence": 0.92,
  "filename": "food.jpg",
  "size_kb": 245
}
```

---

## 🆘 Where to get help

* Open an issue in the GitHub repository
* Check backend API implementation (FastAPI docs)
* Refer to Tailwind CSS documentation for UI customization

Useful links:

* [https://fastapi.tiangolo.com/](https://fastapi.tiangolo.com/)
* [https://tailwindcss.com/docs](https://tailwindcss.com/docs)

---

## 🤝 Contributing

Contributions are welcome! 🎉

Please read the contribution guidelines before submitting a PR:

* [`CONTRIBUTING.md`](docs/CONTRIBUTING.md)

You can help by:

* Improving UI/UX
* Adding calorie or nutrition estimation
* Enhancing ML model accuracy
* Writing tests or documentation

---

## 👤 Maintainer

**Prashanth T**
Computer Science Engineering student
Passionate about AI, ML, and full‑stack development

---

## 📌 Roadmap (Optional Ideas)

* Food calorie estimation
* Portion size detection
* User authentication
* Daily nutrition tracking dashboard
* Mobile‑friendly PWA version

---

⭐ If you find this project useful, consider giving it a star!
