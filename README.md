# Tailwind CSS

## Set Up

**Terminal**

```
npm install -D tailwindcss@3 postcss autoprefixer
```
---
```
npx tailwindcss init -p
```
---

**tailwind.config.js**

```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```
