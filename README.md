
# 🛍️ AndhraCart — Online Shopping Platform

**Live URL:** [https://andhracart.netlify.app/](https://andhracart.netlify.app/)  
**Frontend:** [andhracartview (GitHub)](https://github.com/projectwarriors503/andhracartview)  
**Backend:** [andhracart (GitHub)](https://github.com/projectwarriors503/andhracart)

---

## 🧾 Project Overview

**AndhraCart** is an e-commerce web application built for users to browse products by categories, search, add to cart, and manage user accounts. It features real-time authentication, product management, and responsive design for mobile and desktop users.

---

## 🛠️ Tech Stack

| Layer       | Technologies                                |
|-------------|---------------------------------------------|
| Frontend    | HTML, CSS, JavaScript                       |
| Framework   | Firebase (Firestore, Auth), Supabase (images) |
| Backend     | Python + Flask (hosted on Render)           |
| Hosting     | Netlify (Frontend), Render (Backend API)    |

---

## ✨ Features

- ✅ User registration & login (Firebase Authentication)
- ✅ Responsive product listing
- ✅ Filter by category
- ✅ Add to cart (with user-specific cart in Firestore)
- ✅ Custom popup alerts
- ✅ Mobile bottom navigation
- ✅ Loader with “Please wait…” during fetch
- ✅ Secure backend API for Firebase config (hosted on Render)

---

## 🧩 Folder Structure

### Frontend (`andhracartview`)
\`\`\`
📁 public/
  └── index.html        → Main home page
📁 images/
  └── logo.jpg          → Site icon/logo
📁 js/
  └── logic.js          → Firebase & UI logic
📁 css/
  └── style.css         → Styling rules
\`\`\`

### Backend (`andhracart`)
\`\`\`
📁 app/
  └── main.py           → Flask app with /config route
📁 config/
  └── firebase_config.json  → Hidden secure config
\`\`\`

---

## 🔐 Firebase & Supabase

- **Firebase Firestore** stores:
  - Product data
  - Categories
  - Cart items (per user)
- **Firebase Auth** for login/logout
- **Supabase** used for image storage via public bucket
- **Config API** endpoint delivers Firebase credentials securely (not exposed in frontend)

---

## 🚀 How to Run Locally

### 🧩 Frontend
\`\`\`bash
git clone https://github.com/projectwarriors503/andhracartview
cd andhracartview
# Open index.html in browser
\`\`\`

### ⚙️ Backend (Python)
\`\`\`bash
git clone https://github.com/projectwarriors503/andhracart
cd andhracart
pip install flask flask-cors
python main.py
\`\`\`

Make sure \`firebase_config.json\` is available in backend but **not pushed to GitHub**.

---

## 🐞 Known Issues & Improvements

- ❗Cart data does not persist across logout → Can be extended.
- ❗Admin/product upload UI not yet added.
- 🔧 Add payment gateway integration (e.g., Razorpay)
- 📦 Add order history & checkout page
- 🌙 Add dark mode toggle

---

## 👨‍💻 Contributors

- **Venkata Lakshmi** — UI, Firebase, Logic
- **Your Teammates (if any)** — *(add roles)*

---

## 📄 License

This project is for educational purposes. Feel free to fork and extend it.
