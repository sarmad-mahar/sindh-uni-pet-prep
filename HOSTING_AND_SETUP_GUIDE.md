# 🎓 Sindh University PET Prep Suite - Hosting & Sharing Guide

This application is now structured as an **interactive, mobile-first multi-screen Single Page Application (SPA)**:
- **Screen 1: Paper Selection Dashboard**: Shows all 10 test papers (Past papers 2013–2019 + PET 2025 Mock + High-Yield Model papers), total questions solved, overall average score %, and **last attempt scores & best scores for each individual paper**.
- **Screen 2: Paper Solving Arena**: Mobile-optimized test solver with instant green/red practice feedback, 25-minute exam countdown timer mode, study sheet mode, interactive question palette (`[1] [2]...[25]`) to jump quickly to any question, and touch-friendly MCQ cards.
- **Screen 3: Detailed Scorecard & Review**: Analytical breakdown (English, GK, General Science), passing/merit assessment, question-by-question review (with mistakes-only filter), and one-click WhatsApp / Web Share.

---

## 🚀 How to Host It Online Right Away (Free & Fast)

### Option 1: Netlify Drop (⚡ Fastest — 20 Seconds, No Account Needed)
1. Open your browser and go to: **[app.netlify.com/drop](https://app.netlify.com/drop)**
2. Drag and drop this folder (`Sindh Uni test mock`) into the browser window.
3. Netlify will upload and immediately give you a live HTTPS web address (e.g., `https://random-name-12345.netlify.app`).
4. **Copy that link and send it to your friend on WhatsApp.** They can tap it and solve tests on their Android or iPhone right away!

---

### Option 2: GitHub Pages (Permanent, Free & Custom)
1. Go to **[github.com](https://github.com)** and create a new public repository (e.g. `sindh-university-test-prep`).
2. Upload `index.html` into the repository.
3. Go to repository **Settings** → **Pages** (on the left menu).
4. Under "Branch", select `main` (or `master`), folder `/ (root)`, and click **Save**.
5. Within 1 minute, your site will be live at:
   `https://<your-username>.github.io/sindh-university-test-prep/`

---

### Option 3: Tiiny Host (Single-File Instant Upload)
1. Go to **[tiiny.host](https://tiiny.host)**.
2. Drag and drop `index.html` onto the page.
3. Choose a link name (e.g. `sindh-pet-prep`).
4. Get an instant live link.

---

### Option 4: Direct WhatsApp / File Transfer (100% Offline)
Because `index.html` is completely self-contained (all 250 questions, Tailwind styling, audio synthesizer, and scoring logic are embedded inside):
1. Simply send `index.html` as a **Document** to your friend on WhatsApp or Telegram.
2. Your friend downloads it and taps **"Open with Chrome"** (or Safari).
3. It will work completely offline with zero data consumption!

---

### Option 5: Instant Local Wi-Fi Testing (If on the same Wi-Fi)
If you and your friend are on the same Wi-Fi network:
1. Open PowerShell in this folder and run:
   ```bash
   python -m http.server 8080
   ```
2. Find your PC's local IP address (run `ipconfig`, look for IPv4 e.g. `192.168.1.15`).
3. Tell your friend to open `http://192.168.1.15:8080` in their phone browser.

---

## 📱 Features Built for Mobile & Phones
- **Touch-Friendly Buttons**: Large tap targets (minimum 48px height) designed for thumbs.
- **Quick Jump Palette**: Horizontal scrolling number strip (`1` to `25`) to jump to any question without endless scrolling.
- **Haptic & Sound Effects**: Pleasant audio clicks on selections and celebratory chimes (with a mute button in the header).
- **Persistent Progress**: Scores and attempts stay saved in browser `localStorage`.
- **Add to Home Screen**: On Chrome/Safari, tap "Add to Home Screen" to install it like a native Android/iOS app with no browser URL bar!
