## 🖼️ Image Editor Project - Developer Documentation

### 1. 📌 Project Overview

This project is a **web-based image editor** built using the Toast UI Image Editor. It provides a rich, customizable interface for in-browser image editing. Features include cropping, rotating, drawing, adding shapes, icons, text, masks, and filters. It uses **HTML, CSS, JavaScript**, and is structured for easy local development via `live-server`. The project includes a **custom-styled theme** and loads a default image on startup. Ideal for personal or educational usage.

### 🔗 Project Repository

[GitHub – Toast UI Image Editor (Customized)](https://github.com/Durjoy1971/Toast-UI-Image-Editor)

---

### 2. 🚀 Feature List

| Feature | Description |
| --- | --- |
| Default image load | Loads an image on startup |
| Crop, Flip, Rotate | Basic image transformation tools |
| Freehand Drawing | User can draw with mouse/finger |
| Shapes, Icons, Text | Add elements on canvas |
| Masks & Filters | Apply visual effects |
| Custom UI Theme | Extended theme using `customTheme` |
| Responsive Layout | Works well on desktop browsers |

---

### 3. 🗂️ File & Folder Structure

| File/Folder | Description |
| --- | --- |
| `index.html` | Root HTML page. Includes all necessary scripts and editor container. |
| `app.js` | Initializes the Toast UI Image Editor with custom options and theme. |
| `package.json` | Manages project metadata, dependencies, and live-server script. |
| `.gitignore` | Ignores `node_modules` and other unnecessary files. |

---

### 4. 🧩 Open Source Libraries Used & Customization

- **Toast UI Image Editor**: Core editing tool; heavily customized with a unique theme.
- **Fabric.js** (via CDN): Powers canvas manipulation (internally used by Toast UI).
- **Toast UI Color Picker / Code Snippet** (via CDN): Used for color UI and helper functions.
- **FileSaver.js** (via CDN): Used for saving/exporting edited images.
- **Customization Highlights**:
    - Custom UI styling and icons via the `customTheme` object in `app.js`.
    - Color palette, button styling, and icon overrides for consistency with branding.

---

### 5. ⏱️ Task Estimation

- **Estimated time for a trainee or beginner (without AI):** 3–5 working days
    
    This includes understanding Toast UI basics, setting up the environment, customizing the theme, and testing all core features.
    
- **Estimated time with AI tools (GitHub Copilot, ChatGPT, Claude):** 2–3 working days
    
    AI assistance can speed up setup, provide code examples, clarify API usage, and help troubleshoot errors more quickly.
    

### ⚠️ Challenges

1. **Toast UI Customization**: Documentation is somewhat scattered; deep theme customization is hard without source reading.
2. **CDN Debugging**: Conflicts between local and CDN scripts (e.g., version mismatch).
3. **NPM Tooling**: A beginner might struggle with `npm`, `live-server`, and proper module resolution.
4. **Backward Compatibility**: Toast UI breaks backward compatibility often. AI tools like Copilot/ChatGPT may hallucinate outdated APIs. **Always cross-check with the official docs.**

---

### 6. 🧠 Potential AI Hallucinations / Debugging Notes

| Area | Possible Issue | Debugging Tip |
| --- | --- | --- |
| Toast UI API | AI may reference deprecated or incorrect methods (e.g., `.loadImageFromFile` vs newer method) | Always verify method names in Toast UI docs. |
| Theme Customization | Copilot may ignore valid `customTheme` properties or confuse them with CSS variables | Check the full shape of the `theme` object from official theme API |
| CDN Library Loading | AI may not warn about script loading order conflicts | Always load dependencies like Fabric.js first, then Toast UI, then app.js |
| FileSaver.js Usage | AI may hallucinate `saveAs()` usage without checking the blob type | Check browser compatibility and MIME type when exporting |

---

### 7. 🌱 Suggested Features

1. **Export Options**
    
    Add export settings like image quality (JPEG, PNG), size presets, or PDF export.
    
2. **Drag-and-Drop Upload**
    
    Enable drag-and-drop or drag-from-desktop upload for easier file selection.
    
3. **Multi-format Support**
    
    Support WebP, AVIF, and HEIC formats with fallback and warnings for unsupported browsers.