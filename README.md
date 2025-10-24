# social-networking-platform
# ⚡ Vite React TypeScript Starter

A modern **React + TypeScript** boilerplate built using **Vite**.  
Styled with **Tailwind CSS**, integrated with **Supabase**, and configured for fast development and production builds.

---

## 🧠 Overview

This project provides a clean starting point for building scalable React applications with TypeScript.  
It includes support for Tailwind CSS for rapid UI development and Supabase for backend features such as authentication, database, and storage.

---

## ✨ Features

- ⚛️ **React 18** with **TypeScript**
- ⚡ **Vite 5** for instant builds and hot reloads
- 🎨 **Tailwind CSS 3** with dark mode support
- 🧩 **Supabase JS v2** for backend & authentication
- 🧰 Preconfigured **ESLint**, **TypeScript ESLint**, and **React Refresh**
- 🔄 Ready for deployment to Netlify, Vercel, or any static host

---

## 📁 Folder Structure

```
vite-react-typescript-starter/
├── public/                   # Static assets
├── src/                      # Source files
│   ├── assets/               # Images, fonts, etc.
│   ├── components/           # Reusable UI components
│   ├── App.tsx               # Root component
│   ├── main.tsx              # Entry point
│   └── index.css             # Tailwind base styles
├── index.html                # Main HTML file
├── postcss.config.js         # PostCSS plugins config
├── tailwind.config.js        # Tailwind configuration
├── tsconfig.json             # TypeScript compiler options
├── vite.config.ts            # Vite configuration
└── package.json              # Project metadata & dependencies
```

---

## 🧰 Tech Stack

| Tool | Description |
|------|--------------|
| [React](https://react.dev/) | Frontend library for building UI |
| [TypeScript](https://www.typescriptlang.org/) | Type-safe JavaScript |
| [Vite](https://vitejs.dev/) | Next-gen frontend build tool |
| [Tailwind CSS](https://tailwindcss.com/) | Utility-first CSS framework |
| [Supabase](https://supabase.io/) | Backend as a Service (Auth, DB, Storage) |
| [ESLint](https://eslint.org/) | Code linting |
| [Lucide React](https://lucide.dev/) | Icon library |

---

## 🚀 Getting Started

### 1️⃣ Prerequisites
Make sure you have:
- **Node.js** (v18 or higher)
- **npm** or **yarn**

Check versions:
```bash
node -v
npm -v
```

---

### 2️⃣ Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/your-username/vite-react-typescript-starter.git
cd vite-react-typescript-starter
npm install
```

---

### 3️⃣ Running the Development Server

Start the app locally:

```bash
npm run dev
```

Then open in your browser:
👉 **http://localhost:5173**

---

### 4️⃣ Build for Production

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

---

### 5️⃣ Lint and Type Check

Run ESLint:
```bash
npm run lint
```

Run TypeScript type checking:
```bash
npm run typecheck
```

---

## ⚙️ Environment Variables

To use Supabase, create a `.env` file in your project root:

```bash
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_ANON_KEY=your-anon-key
```

Access these in your app:
```ts
import { createClient } from '@supabase/supabase-js';

const supabase = createClient(
  import.meta.env.VITE_SUPABASE_URL!,
  import.meta.env.VITE_SUPABASE_ANON_KEY!
);
```

---

## 🎨 Tailwind CSS Setup

Configured via `tailwind.config.js`:

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  darkMode: 'class',
  theme: {
    extend: {},
  },
  plugins: [],
};
```

You can toggle dark mode by adding or removing the `class="dark"` on the `<html>` tag.

---

## 🧩 Example Component

```tsx
import { useState } from 'react';

function App() {
  const [count, setCount] = useState(0);

  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-gray-50 dark:bg-gray-900 text-center">
      <h1 className="text-3xl font-bold mb-4 text-blue-600">Vite + React + TypeScript</h1>
      <p className="text-lg mb-4">Count: {count}</p>
      <button
        onClick={() => setCount(count + 1)}
        className="px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600"
      >
        Increment
      </button>
    </div>
  );
}

export default App;
```

---

## 🧠 Common Scripts

| Command | Description |
|----------|--------------|
| `npm run dev` | Start development server |
| `npm run build` | Build production files |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint checks |
| `npm run typecheck` | Verify TypeScript types |

---

## 🧰 Troubleshooting

If you see errors like `"Cannot find module 'react'"`:
1. Run `npm install` again  
2. Ensure file extension is `.tsx` (for TypeScript)  
3. Restart TypeScript server → Press `Ctrl + Shift + P` → *Restart TS Server*

---

## 💡 Deployment

You can easily deploy to:

- [Vercel](https://vercel.com/)
- [Netlify](https://www.netlify.com/)
- [GitHub Pages](https://pages.github.com/)
- [Render](https://render.com/)

For example (Vercel):
```bash
npm run build
vercel deploy
```

---

## 🧑‍💻 Author

**Your Name**  
📧 [c.harini1109@gmail.com]  
🌐 [https://www.artfolio.tech/harini_c?edit=false]  
---

## 📜 License

This project is licensed under the **MIT License** — you are free to use, modify, and distribute it.

---
