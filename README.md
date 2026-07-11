# Connect 4 & 5 AI Solver 🎮

An optimized, zero-dependency, mobile-first Connect 4 and Connect 5 web application featuring a high-performance adversarial AI solver engine. Built entirely in a single, lightweight HTML5/JavaScript file tailored for offline performance on iOS and mobile devices.

## 🚀 Live Demo
Play the game instantly in your mobile or desktop browser:
👉 **[Deploy Your Link Here After Setup]**

---

## ✨ Features
*   **Dual Mode Engine:** Toggle seamlessly between classic **Connect 4 (7x6 Grid)** and custom **Connect 5 (9x7 Grid)** setups.
*   **Flexible Player Matching:** Configure matchups dynamically (Human vs. AI, AI vs. AI, or local Pass-and-Play).
*   **Optimized Mobile Performance:** Implements asynchronous thread-yielding (`requestAnimationFrame`) to prevent WebKit script execution timeouts on mobile processors.
*   **Responsive Fluid Layout:** Uses modern CSS layouts (`clamp()`, `vmax`, and Grid) to autoscale to edge-to-edge fullscreen perfection on iPhones and iPads.

---

## 🧠 AI Solver Architecture
The underlying AI solver does not rely on random simulations or external server requests. It uses classical game theory algorithms optimized for fast execution:

1. **Minimax Algorithm:** Simulates potential future outcomes up to several turns ahead by alternating between maximizing the AI's score and minimizing the opponent's options.
2. **Alpha-Beta Pruning:** Dramatically reduces execution time by trimming branches in the game tree that are mathematically proven to yield worse results than previously evaluated paths.
3. **Dynamic Positional Matrix:** Scores individual token placements using a dynamic center-weighted heuristic map—incentivizing control over critical middle structural columns.
4. **Deterministic Lookaheads:** Intercepts deep calculations to immediately seize instant wins or block incoming opponent fatal checkmates in $O(N)$ execution time.

---

## 🛠️ Local Installation & iOS Offline Use
Since the entire application is self-contained in a single file, you can run it completely offline.

### Running Locally (Mac/PC/Linux)
1. Clone this repository: `git clone https://github.com/z3nax/connect-solver.git`
2. Open `index.html` directly in any web browser.

### Running Offline on iPhone/iPad
1. Open the live deployment link in **Safari**.
2. Tap the **Share** button (the arrow box icon at the bottom center).
3. Scroll down and select **Add to Home Screen**.
4. The game will now appear as an app icon on your home screen and will launch instantly—even if you are in Airplane Mode with zero cellular service.

---

## 📄 License
This project is open-source and free to use under the MIT License.

Developed by [z3nax](https://github.com/z3nax).
