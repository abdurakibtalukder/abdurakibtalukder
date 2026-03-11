# 🌗 Auto Device Theme Preference

Automatically adapts to your device's **dark** or **light** mode in real time — no user input required.

---

## ✨ Features

- 🔄 **Auto theme detection** — reads the OS/browser `prefers-color-scheme` setting on load
- 🌙 **Dark mode** — activated when device is in dark mode
- ☀️ **Light mode** — activated when device is in light mode
- ⚡ **Live switching** — theme changes instantly when you toggle your device setting, no page reload needed
- 🎨 **CSS custom properties** — all colors are driven by variables for easy customization
- ♿ **Accessible** — follows system intent, respects user preferences

---

## 🚀 Quick Start

### HTML / CSS

```html
<!-- Link your stylesheet -->
<link rel="stylesheet" href="theme.css" />
```

```css
/* theme.css */
:root {
  --bg: #ffffff;
  --text: #111111;
  --accent: #0066ff;
  --surface: #f4f4f4;
}

@media (prefers-color-scheme: dark) {
  :root {
    --bg: #0d0d0d;
    --text: #f0f0f0;
    --accent: #66aaff;
    --surface: #1a1a1a;
  }
}

body {
  background-color: var(--bg);
  color: var(--text);
}
```

### JavaScript — Live Listener

```js
const mq = window.matchMedia('(prefers-color-scheme: dark)');

function applyTheme(isDark) {
  document.documentElement.setAttribute(
    'data-theme',
    isDark ? 'dark' : 'light'
  );
}

// Apply on load
applyTheme(mq.matches);

// React to OS changes in real time
mq.addEventListener('change', (e) => applyTheme(e.matches));
```

### React Hook

```jsx
import { useState, useEffect } from 'react';

export function useAutoTheme() {
  const mq = window.matchMedia('(prefers-color-scheme: dark)');
  const [isDark, setIsDark] = useState(mq.matches);

  useEffect(() => {
    const handler = (e) => setIsDark(e.matches);
    mq.addEventListener('change', handler);
    return () => mq.removeEventListener('change', handler);
  }, []);

  return isDark ? 'dark' : 'light';
}
```

---

## 🎨 CSS Variable Reference

| Variable     | Light Mode  | Dark Mode   | Usage              |
|--------------|-------------|-------------|--------------------|
| `--bg`       | `#ffffff`   | `#0d0d0d`   | Page background    |
| `--text`     | `#111111`   | `#f0f0f0`   | Body text          |
| `--accent`   | `#0066ff`   | `#66aaff`   | Buttons, links     |
| `--surface`  | `#f4f4f4`   | `#1a1a1a`   | Cards, panels      |
| `--border`   | `#dddddd`   | `#2a2a2a`   | Dividers, outlines |
| `--muted`    | `#888888`   | `#666666`   | Subtle text        |

---

## 🗂 File Structure

```
project/
├── index.html       ← Main HTML entry
├── theme.css        ← CSS custom properties & media query
├── theme.js         ← Optional JS listener for live switching
└── README.md        ← You are here
```

---

## 🔧 How It Works

1. **CSS `@media (prefers-color-scheme: dark)`** — the browser exposes the OS theme as a media query. CSS variables inside this block automatically override the `:root` defaults.
2. **`window.matchMedia()`** — JavaScript can read and *listen* to the same media query, letting you apply classes, attributes, or state changes the moment the device theme changes.
3. **No flash** — because CSS loads before paint, the correct theme is applied instantly with zero flicker.

---

## 🌍 Browser Support

| Browser        | `prefers-color-scheme` | Live `change` event |
|----------------|------------------------|---------------------|
| Chrome 76+     | ✅                      | ✅                   |
| Firefox 67+    | ✅                      | ✅                   |
| Safari 12.1+   | ✅                      | ✅                   |
| Edge 79+       | ✅                      | ✅                   |
| iOS Safari 13+ | ✅                      | ✅                   |

---

## 📄 License

MIT — free to use and modify.




```js
class Philosophy {
  life() {
    return 'Life is limited. Time will not wait.';
  }

  mindset() {
    return 'Every "no" is the next opportunity — keep moving.';
  }

  growth() {
    return 'Learn daily. Improve constantly. Stay curious.';
  }

  mission() {
    return 'Build clean, useful, and meaningful things.';
  }

  purpose() {
    return 'Make life better — even in small ways.';
  }
}

export default new Philosophy();
```
