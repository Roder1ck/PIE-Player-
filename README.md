# 🥧 PIE Player
**Programmable Integrated Exhibition Player**

PIE Player is a lightweight, web-native digital signage solution designed for simplicity, speed, and seamless performance. Built with a "Zero-Backend" philosophy, PIE Player allows users to transform any browser-enabled screen into a professional advertisement display without the need for complex software installations, databases, or monthly subscriptions.

---

## 📖 Description
The **PIE Player** (Programmable Integrated Exhibition Player) is an "out-of-the-box" advertisement loop system. It leverages modern web technologies to provide a high-quality visual experience. By separating the management logic from the presentation layer, it allows for real-time updates to a live display from a secondary control device.

Whether you are running a menu board in a café, a welcome screen in a corporate lobby, or a promotional kiosk in a retail store, PIE Player makes digital signage **as easy as pie.**

---

## 🚀 Key Features

*   **Dual-Page Architecture**: 
    *   **The Kitchen (Manager):** A clean UI to structure your playlist, add media URLs, and set timing.
    *   **The Plate (Display):** A distraction-free, full-screen playback environment.
*   **Intelligent Media Handling**:
    *   **Images**: Customizable duration timers for static content.
    *   **Videos**: Smart "End-of-File" detection that automatically transitions to the next ad once the video finishes.
*   **Cinematic Transitions**: Features hardware-accelerated **Fade-In/Fade-Out** animations, ensuring a smooth, premium feel between advertisements.
*   **Instant-Sync Technology**: Uses the browser's `StorageEvent` API. When you save changes in the Manager, the Display page updates **instantly** without needing a page refresh.
*   **Pure Vanilla Stack**: Built 100% with HTML5, CSS3, and JavaScript. No external libraries, no dependencies, and no server-side processing required.

---

## 🛠️ How It Works

1.  **Local Environment**: The program runs entirely in the browser. It uses `localStorage` to store your playlist data locally on the machine.
2.  **The Loop**: Once a playlist is "Baked" (Saved), the Display page enters a continuous loop. 
3.  **Handoff Logic**: 
    *   For **Images**, the JavaScript `setTimeout` function handles the transition. 
    *   For **Videos**, the `onended` event listener ensures that the next ad starts the millisecond the current video stops.

---

## 📂 File Structure

*   `manage.html` - The configuration dashboard where you build your playlist.
*   `display.html` - The output screen (designed to be viewed on the primary display).

---

## 📥 Installation & Setup

1.  Download or copy the `manage.html` and `display.html` files into the same folder.
2.  Open `display.html` in your browser. (Tip: Press `F11` for full-screen mode).
3.  Open `manage.html` in a separate tab or on a different monitor.
4.  Enter your media URLs (Direct links to `.jpg`, `.png`, `.mp4`, etc.).
5.  Click **Apply & Save** and watch the transition happen instantly on the display.

---

**PIE Player** — *Cinematic signage simplified.*
