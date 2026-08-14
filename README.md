
# MedQ Local — Offline Question Bank

**MedQ Local** is a client-side web application designed for building, managing, and practicing custom question banks completely offline. Built with zero external library dependencies, it runs directly inside any modern web browser, keeping your study data private and fast.


---
## 🌟 Key Features

* **100% Offline & Private**: All study records, questions, bookmarks, and settings stay on your machine without transmitting data across the internet.
* **Dual Storage Options**: Store data in browser storage or connect directly to a local `.json` project file via the File System Access API to avoid storage caps.
* **Practice & Timed Exam Modes**: Configure customizable practice sessions or timed tests complete with countdown timers, option shuffling, and configurable question counts.
* **Custom Quiz Workspace**: Tailor your practice session with adjustable text sizes (A- / A+), container widths (narrow, standard, wide), compact density layouts, and a collapsible question navigator.
* **Multi-Format Importing**: Import question sets seamlessly from JSON, CSV, Markdown (`.md`), or TXT formats with automatic duplicate ID protection.
* **Rich Media & SVG Charts**: Attach local images to questions and explanations, or render dynamic SVG bar and line graphs.
* **Analytics & Performance Insights**: Track study trends using daily activity heatmaps, accuracy scores, streak counters, average response times, and dedicated wrong-answer review queues.
* **Subject & Tag Management**: Organize questions by categories and tags, and use the built-in Subject Manager to rename, merge, or migrate topics across questions.
* **Custom Course Branding**: Personalize the sidebar and dashboard labels (e.g., "Medical student years 1–3" or exam titles).

---

## 🛠 Tech Stack

* **HTML5**: Semantic web markup.
* **CSS3**: Modern responsive layout using CSS Grid, Flexbox, dynamic CSS variables, and media queries.
* **Vanilla JavaScript (ES6+)**: Zero third-party dependencies, leveraging native browser APIs (Local Storage & File System Access API).

---

## 🚀 Getting Started

Because **MedQ Local** is packaged as a single standalone application, setup is instant:

1. **Clone or Download** this repository.
2. **Open `index.html`** in any modern web browser (e.g., Chrome, Edge, Brave).
3. **Start practicing** immediately using the built-in sample questions or import your own datasets.

---

## 📄 File Import Specifications

MedQ Local supports importing question banks through multiple file formats:

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

```

### 2. CSV Format

Expected headers:
`id,question,option_a,option_b,option_c,option_d,answer,explanation,references,subject,tags,image,image_alt,image_caption,chart_type,chart_title,chart_labels,chart_values`

### 3. Markdown / TXT Format

Separate individual questions using `---` dividers and key markers like `# Q001`, `Question:`, `A.`, `Answer:`, `Image:`, and `Chart Type:`.

---

## 🔒 Privacy & Data Control

* **Zero External Calls**: No analytics, tracking scripts, or cloud servers are embedded in the application.
* **Data Portability**: Full backup archives can be exported or restored at any time from the settings menu.

---

## 📜 License

This project is licensed under a **Personal & Non-Commercial Use License** — free to use, modify, and study for individual non-commercial purposes. Commercial use and public redistribution are strictly prohibited. See the [LICENSE] file for details.

```
