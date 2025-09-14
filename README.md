# 🧠 Digital Mental Health Support System

This project is a **prototype web application** designed for students to access digital mental health support, submit feedback, and manage simple interactions with doctors and professionals.  

It consists of several HTML pages connected through forms and navigation.

---

## 📂 Project Structure

- **Register.html**  
  Registration page for new users. Collects name and age before redirecting to the login page.  
  ➝ Form action: `login page.html`

- **login page.html**  
  Login page for registered users. Collects **email** and **password**. On success, redirects to the main app page.  
  ➝ Form action: `app1.html`

- **app1.html**  
  Home page (main dashboard).  
  - Allows users to **report a problem**.  
  - Provides a dropdown menu with options (timetable, doctors, professionals, calls, messages).  
  - Displays selected content inside an `<iframe>`.  

- **timetable.html**  
  A form where users can input suggestions from doctors or department professionals.  
  ➝ Submits data to a placeholder API endpoint.

- **review submission.html**  
  Collects student reviews:  
  - Student App ID  
  - Rating (1–5)  
  - Comments  
  Displays review results and stores them in `localStorage`.

---

## 🚀 How to Run

1. Download or clone the project.
2. Place all `.html` files in the same folder.
3. Open `Register.html` in a web browser to start the flow:
   - Register → Login → Dashboard (`app1.html`)
4. Use the dropdown in `app1.html` to navigate to other features.

---

## ⚙️ Features (Prototype)

- User **registration and login** flow.
- Problem **reporting form**.
- **Timetable suggestion form** for doctors and professionals.
- **Review submission** with local storage saving.
- Simple **iframe-based navigation** between modules.

---

## 🛠️ Improvements Needed

- **Form IDs missing**: JavaScript event listeners won’t work unless forms have `id` attributes (`registerForm`, `loginForm`, `reviewForm`, `timetableForm`).  
- **Backend APIs**: Currently use placeholder endpoints (`https://example.com/api/...`). Replace with actual backend URLs.  
- **Security**: No password validation or encryption yet.  
- **UI/UX**: Pages can be redesigned with consistent styling, navigation bar, and responsive layout.  
- **Validation**: Input fields should be validated (e.g., rating between 1–5, required comments, etc.).

---

## 📌 Next Steps

1. Add **form IDs** to make JavaScript work properly.  
2. Connect to a **real backend API** for storing reports, reviews, and timetable suggestions.  
3. Implement **database support** (e.g., MySQL, Firebase, or MongoDB).  
4. Enhance UI with CSS framework (Bootstrap/Tailwind).  
5. Add **session management** for logged-in users.

---

## 👨‍💻 Author
Prototype developed for a **Digital Mental Health App for Students** project.
