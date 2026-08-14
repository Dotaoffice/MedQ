# MedQ
MedQ Local is an offline-first, client-side question bank and quiz study workspace built for medical students and self-learners. It features complete local privacy, JSON project file integration, multi-format file importing (JSON/CSV/Markdown/TXT), timed exam modes, dynamic SVG charts, and interactive study analytics.
# MedQ Local — Offline Question Bank

**MedQ Local** is a client-side web application designed for building, managing, and practicing custom question banks completely offline. Built with zero external library dependencies, it runs directly inside any modern web browser, keeping your study data private and fast.

---

## 🌟 Key Features

* **100% Offline & Private**: All study records, questions, bookmarks, and settings stay on your machine without transmitting data across the internet.
* **Dual Storage Options**: Store data in browser storage or connect directly to a local `.json` project file via the File System Access API to avoid storage caps.
* **Practice & Timed Exam Modes**: Configure customizable practice sessions or timed tests complete with countdown timers, option shuffling, and configurable question counts[cite: 1].
* **Custom Quiz Workspace**: Tailor your practice session with adjustable text sizes ($A- / A+$), container widths (narrow, standard, wide), compact density layouts, and a collapsible question navigator[cite: 1].
* **Multi-Format Importing**: Import question sets seamlessly from JSON, CSV, Markdown (`.md`), or TXT formats with automatic duplicate ID protection[cite: 1].
* **Rich Media & SVG Charts**: Attach local images to questions and explanations, or render dynamic SVG bar and line graphs[cite: 1].
* **Analytics & Performance Insights**: Track study trends using daily activity heatmaps, accuracy scores, streak counters, average response times, and dedicated wrong-answer review queues[cite: 1].
* **Subject & Tag Management**: Organize questions by categories and tags, and use the built-in Subject Manager to rename, merge, or migrate topics across questions[cite: 1].
* **Custom Course Branding**: Personalize the sidebar and dashboard labels (e.g., "Medical student years 1–3" or exam titles)[cite: 1].

---

## 🛠 Tech Stack

* **HTML5**: Semantic web markup[cite: 1].
* **CSS3**: Modern responsive layout using CSS Grid, Flexbox, dynamic CSS variables, and media queries[cite: 1].
* **Vanilla JavaScript (ES6+)**: Zero third-party dependencies, leveraging native browser APIs (Local Storage & File System Access API)[cite: 1].

---

## 🚀 Getting Started

Because **MedQ Local** is packaged as a single standalone application, setup is instant[cite: 1]:

1. **Clone or Download** this repository[cite: 1].
2. **Open `index.html`** in any modern web browser (e.g., Chrome, Edge, Brave)[cite: 1].
3. **Start practicing** immediately using the built-in sample questions or import your own datasets[cite: 1].

---

## 📄 File Import Specifications

MedQ Local supports importing question banks through multiple file formats[cite: 1]:

### 1. JSON Format
```json
[
  {
    "id": "Q001",
    "question": "Question text stem",
    "options": { "A": "First option", "B": "Second option" },
    "answer": ["A"],
    "explanation": "Detailed rationale",
    "references": ["Reference or textbook source"],
    "subject": "Subject Name",
    "tags": ["Chapter", "Topic"],
    "image": { "src": "data:image/png;base64,...", "alt": "Anatomy diagram", "caption": "Optional caption" },
    "chart": { "type": "bar", "title": "Chart Title", "labels": ["A", "B"], "values": [12, 19] }
  }
]
