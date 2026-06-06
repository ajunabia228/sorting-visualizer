# 📊 Sorting Visualizer

An interactive, side-by-side sorting algorithm visualizer built with vanilla HTML, CSS, and JavaScript 📈<br> 
All no frameworks, no build step, one file 📁

<p align="center">
  <img src="screenshots/mainmenu.png" width="60%" alt="main menu screen" />
</p>

<p align="center">
  <a href="https://ajunabia228.github.io/sorting-visualizer">
    <img src="https://img.shields.io/badge/▶%20TEST%20IT%20LIVE-00ff88?style=for-the-badge&logoColor=black" alt="Test it live">
  </a>
</p>

---

## 🛠️ Features

- **9 algorithms**: animated simultaneously (Bubble, Insertion, Selection, Merge, Quick Sort, Heap, Shell, Radix, Tim)
- **Quick Start menu**: pick algorithms, array type, size, and speed before launching
- **Best / Worst / Random case toggle**: see how nearly-sorted or reverse-sorted input affects each algorithm in real time
- **Live complexity graph**: Chart.js line chart plotting cumulative comparisons vs steps; O(n²) curves diverge visibly from O(n log n) ones
- **Color-coded bar states**: comparing (amber), swapping (red), pivot (purple), selected/min (pink), sorted (green)
- **Presets**: O(n²) trio, O(n log n) trio, All 9, Quick Sort worst case, Shell + Radix + Tim
- **Adjustable array size**: (10–60 elements) and 5 speed levels
- **Dark mode** support via `prefers-color-scheme`
- Zero dependencies at runtime: Chart.js loaded from CDN, Tabler icons via CDN

---

## 🔢 Algorithms

<p align="center">
  <img src="screenshots/sorting.png" width="60%" alt="sorting screen" />
</p>

| Algorithm      | Best case   | Average     | Worst case  | Space  | Stable? |
|----------------|-------------|-------------|-------------|--------|---------|
| Bubble sort    | O(n)        | O(n²)       | O(n²)       | O(1)   | Yes     |
| Insertion sort | O(n)        | O(n²)       | O(n²)       | O(1)   | Yes     |
| Selection sort | O(n²)       | O(n²)       | O(n²)       | O(1)   | No      |
| Merge sort     | O(n log n)  | O(n log n)  | O(n log n)  | O(n)   | Yes     |
| Quick Sort     | O(n log n)  | O(n log n)  | O(n²)       | O(log n)| No      |
| Heap sort      | O(n log n)  | O(n log n)  | O(n²)  | O(1)   | No      |
| Shell sort      | O(n log n)  | O(n log² n)*  | O(n²)*  | O(1)   | No |
| Radix sort      | O(d * (n + k))  | O(d(n + k))  | O(d(n + k))  | O(n + k)   | Yes |
| Tim sort      | O(n)  | O(n log n)  | O(n log n)  | O(n)   | Yes |

<sub><sub>*Shell Sort complexities vary significantly based on the mathematical gap sequence implemented</sub></sub>


---

## 🏁 Getting Started

### Run locally

No install needed. Just open the file:

```bash
git clone https://github.com/ajunabia228/sorting-visualizer.git
cd sorting-visualizer
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or serve it with any static server:

```bash
npx serve .
# → http://localhost:3000
```

---

## 🏗️ Project Structure

```
sorting-visualizer/
├── index.html      # entire app — HTML, CSS, and JS in one file
└── README.md
```

---

## 💻 Tech Stack

- **Vanilla JS**: all sorting logic and animation
- **Chart.js 4**: complexity graph (loaded from CDN)
- **Tabler Icons**: UI icons (loaded from CDN)
- **CSS custom properties**: theming and dark mode
- **GitHub Pages**: hosting

---

## 🪪 License

This project is free to use, fork, and build on under the [MIT License](LICENSE).
