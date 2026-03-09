# InstagramParser
Convert Instagram message export HTML into a persistent todo list for processing links.


A lightweight browser tool that converts **Instagram message export HTML** into a **persistent todo list** for processing shared links.

Designed for workflows where each message needs manual handling — such as opening links, taking screenshots, archiving content, or migrating data into another application.

Everything runs **locally in your browser**. No backend required.

---

## Features

- Parse Instagram message export HTML
- Extract Instagram post / reel links
- Convert messages into actionable todo items
- Mark tasks complete
- Attach screenshots to tasks
- Local persistence using `localStorage`
- Export tasks as:
  - JSON
  - CSV
  - Markdown
- Drag-and-drop screenshot support (desktop)
- Works offline

---

## Example Workflow

1. Export Instagram messages
2. Load the export HTML into the tool
3. Each message becomes a todo task
4. Open the link
5. Capture screenshot
6. Attach screenshot to the task
7. Mark task complete
8. Export processed tasks to another system

---

## Screenshot Workflow

```
Instagram Export
      ↓
HTML Parser
      ↓
Todo List
      ↓
Open Link → Screenshot → Attach
      ↓
Mark Complete
      ↓
Export
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/instagram-export-todo.git
```

Navigate into the project:

```bash
cd instagram-export-todo
```

Open the app:

```
open ig-todo.html
```

Or simply double-click the HTML file.

No build step required.

---

## Usage

### 1. Load Instagram Export

Click **Load Export** and select the Instagram HTML export file.

Or paste the HTML directly into the interface.

---

### 2. Process Tasks

Each detected Instagram link becomes a task.

For each task:

1. Click the link
2. Capture screenshot
3. Attach screenshot
4. Mark task done

---

### 3. Export Results

The processed list can be exported as:

| Format | Use Case |
|------|------|
JSON | programmatic processing |
CSV | spreadsheets / bulk import |
Markdown | documentation / notes |

---

## Mobile Usage

The tool works on **mobile Chrome**, though desktop offers the best experience.

Recommended mobile workflow:

1. Open the tool
2. Load export
3. Open link
4. Take screenshot
5. Attach screenshot
6. Mark done

For better persistence, host the file (GitHub Pages, Netlify, etc.).

---

## Data Storage

All data is stored locally using:

```
localStorage: ig_todo_v1
```

No external services or analytics are used.

Your data never leaves your device.

---

## Supported Instagram Links

The parser detects:

- Posts  
- Reels  
- IGTV links

Example:

```
instagram.com/p/
instagram.com/reel/
instagram.com/tv/
```

---

## Limitations

- Parsing depends on the Instagram export HTML structure
- Screenshot capture is manual
- Large exports may take a moment to parse

---

## Possible Improvements

- Automatic screenshot capture via Puppeteer
- Browser extension for direct capture
- Cloud sync support
- Tagging and filtering
- Progress dashboard
- PWA installable version
- Multi-user support

---

## Contributing

Pull requests are welcome.

If you want to improve parsing reliability or extend export options, feel free to open an issue first to discuss.

---

## License

MIT License
