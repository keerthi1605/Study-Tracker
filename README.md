# Study-Tracker
Perfect, Kee 👍 you don’t want to juggle **frontend + backend + DB + AI + realtime** all at once — that’s where people burn out.
We’ll **layer the project in parts** so every step adds something new and feels complete.

---

# 📌 Development Parts (Slow & Steady)

### **Part 1: UI Mock + Static Frontend (React only)**

🎯 *Goal:* Just design how the app looks — no backend.

* Setup React + Tailwind project.
* Build pages/components:

  * Login / Signup (just static inputs & buttons).
  * Dashboard with:

    * Subject list.
    * Pomodoro timer UI.
    * Placeholder heatmap.
    * Stats card (dummy values).
* Navigation with React Router.
* No real data → use **dummy JSON** inside components.

✅ At the end: You can click around, timer UI runs locally, fake data shows up.

---

### **Part 2: Backend Setup (Express + MongoDB)**

🎯 *Goal:* Make your static UI talk to a real backend.

* Setup Express server + MongoDB Atlas.
* Build REST APIs for:

  * Auth (Signup/Login).
  * Subjects (CRUD).
  * Study sessions (log sessions).
* Connect React UI → Axios fetch from APIs.
* Implement login flow → store JWT in localStorage.

✅ At the end: You have working login, subjects saved to DB, and sessions stored.

---

### **Part 3: Pomodoro Timer + Session Logging**

🎯 *Goal:* Make Pomodoro useful.

* Hook timer → when session completes, POST to backend `/api/sessions`.
* Store `start`, `end`, `duration`, `subject`.
* Update frontend dashboard to show today’s logged sessions from DB.

✅ At the end: Study time actually gets saved and displayed.

---

### **Part 4: Analytics + Heatmap**

🎯 *Goal:* Add insights.

* Backend aggregation API → total minutes per day.
* React heatmap component (react-calendar-heatmap).
* Charts: subjects vs hours (Recharts).

✅ At the end: User sees progress visualized instead of raw numbers.

---

### **Part 5: Gamification (XP, streaks, badges)**

🎯 *Goal:* Make it fun.

* Add XP system in backend (formula).
* Calculate streaks.
* Display progress bar + badges in frontend profile page.

✅ At the end: Studying feels rewarding with visible progress.

---

### **Part 6: AI Study Coach**

🎯 *Goal:* Add brains 🤖.

* Use OpenAI (or similar API).
* Backend endpoint → fetch user’s last sessions, send prompt to AI, return study plan.
* Frontend: “Get AI Plan” button → shows personalized plan/tips.

✅ At the end: App gives smart suggestions, not just tracking.

---

### **Part 7: Social / Accountability (optional, advanced)**

🎯 *Goal:* Add collaboration.

* Implement Socket.io.
* “Study Together” room → shared Pomodoro timer + live chat.
* Friend leaderboard or buddy streak system.

✅ At the end: Feels like a social learning hub, not a solo app.

---

### **Part 8: PWA + Offline Mode**

🎯 *Goal:* Make it work anywhere.

* Convert React app into PWA (manifest + service worker).
* Store sessions offline in IndexedDB.
* Sync with server when online.

✅ At the end: Even without internet, user can study & sync later.

---

# 🛠 Order Recap:

1. **UI (Frontend mock)** → just visuals.
2. **Backend basics** → auth + DB storage.
3. **Pomodoro logging** → sessions saved.
4. **Analytics (heatmap, charts)** → insights.
5. **Gamification** → XP, streaks, badges.
6. **AI tips** → study coach.
7. **Social features** (optional advanced).
8. **Offline/PWA** polish.

---

👉 This way you **learn React → API → DB → analytics → AI → realtime → offline** step by step. Each part is a mini-project on its own.

Do you want me to **start with Part 1 (UI mock)** and give you the exact React folder structure + first components (login, dashboard, timer placeholder) so you can begin coding right away?
