# 🏁 Track Command
### The High-Visibility Garage Dashboard for Track Days & Racing

**Track Command** is a lightweight, client-side web application designed to be the "digital pit wall" for your garage. Built specifically for motorcycle track days (NEMRR, Jennings GP, etc.), it provides a high-contrast, massive-font countdown to your next session, so you can see your status from across the paddock while wrenching or geared up.

---

## 🚀 Key Features

* **Dynamic Split-Screen:** Toggle between a massive single-rider view or a perfectly equitable 50/50 split-screen for you and a teammate.
* **Pro Alert Logic:** Four independent, color-coded states that change the entire screen background for "at-a-glance" status updates:
    * **Riders Meeting:** A dedicated morning countdown to the briefing.
    * **Warmup Alert:** Reminds you to start engines and check tire warmers.
    * **Gear Up Alert:** The "Final Call" to get your suit, boots, and helmet on.
    * **Stand Prep (Session Ending):** A blinking alert that triggers near the end of a session so you can have the rear stands and warmers ready in the hot pit.
* **Custom Branding:** Personalize the dashboard with your Team Name, Race Number, and custom labels for each rider.
* **Fully Themeable:** Every alert state has a configurable color picker to match your bike’s livery or your personal preference.
* **Zero Infrastructure:** A single `.html` file that runs entirely in the browser. No server, no database, no internet required.
* **Offline Persistence:** All configurations are saved to your browser's `LocalStorage`. Close the tab or reboot your laptop; your schedule and colors stay put.

---

## 🛠 How to Use

1.  **Launch:** Open `index.html` in any modern web browser (Chrome, Safari, Firefox).
2.  **Configure:** Click the **Gear Icon** in the top-right corner to open the Settings.
3.  **Set Your Rotation:**
    * Pick your **1st Session Hour** (usually 09:00).
    * Choose your **Rotation Length** (15 or 20 minutes).
    * Select your **Group Slot** (e.g., if you are the 2nd group out, choose `:20`).
4.  **Customize Alerts:** Turn on the alerts you need and set your preferred lead times (e.g., 10m for Warmup, 5m for Gear Up).
5.  **Save:** Hit **Apply All Changes**. The app will automatically build your schedule for the entire day, including a lunch-break blackout.

---

## 💻 Developer & Testing Tools

Testing a track day schedule at 10:00 PM in your living room is difficult. We’ve included a **Debug Override** feature:
* Enable **"Debug Override"** in the Advanced section.
* Input a "System Time" close to a session start (e.g., if your session is at 09:00, set debug to 08:52:00).
* The app will treat the override time as "Now," allowing you to watch the transitions between Warmup, Gear Up, and On Track states in real-time.

---

## 📋 Tech Stack

* **HTML5 / CSS3:** Custom Flexbox/Grid layout with CSS Variables for theming.
* **Vanilla JavaScript:** No frameworks or external dependencies.
* **Font Awesome:** Included via CDN for icons.
* **Persistence:** `window.localStorage` for data retention.

---

## 🏁 Credits & License
Created for the track community. Free to use, modify, and distribute. 

**Ride fast. Have Fun. Don't miss your session.** 🏍️💨