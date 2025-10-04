# 🛠️ Tailwind CSS Setup Guide

This guide will help you set up Tailwind CSS for your web development projects in the simplest way possible. Choose the method that fits your needs!

---

## 1️⃣ Easiest: Use Tailwind via CDN (Recommended for Simple Projects)

Just add the following line inside the `<head>` of your HTML file:

```html
<script src="https://cdn.tailwindcss.com"></script>
```

- No installation required.
- Great for quick demos and assignments.
- All Tailwind utility classes are available.

---

## 2️⃣ Local Tailwind Setup (For Advanced/Custom Projects)

If you want to use custom Tailwind configuration, plugins, or build tools, follow these steps:

### Step 1: Initialize Your Project

```bash
npm init -y
```

### Step 2: Install Tailwind CSS

```bash
npm install -D tailwindcss
npx tailwindcss init
```

### Step 3: Configure Tailwind

Edit your `tailwind.config.js` and set the `content` paths to include your HTML files:

```js
module.exports = {
  content: ["./*.html", "./**/*.html"],
  theme: { extend: {} },
  plugins: [],
};
```

### Step 4: Create Your CSS File

Create a file like `styles.css` and add:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Step 5: Build Your CSS

```bash
npx tailwindcss -i ./styles.css -o ./output.css --watch
```

- Link `output.css` in your HTML `<head>`.
- Now you can use all Tailwind classes!

---

## 3️⃣ Try Online: Tailwind Play

- Use [Tailwind Play](https://play.tailwindcss.com/) for instant prototyping in your browser.

---

## 📚 Resources

- [Tailwind CSS Documentation](https://tailwindcss.com/docs/installation)
- [Tailwind Play](https://play.tailwindcss.com/)

---

Happy styling with Tailwind CSS! 🎨
