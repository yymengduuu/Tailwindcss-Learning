# Tailwind CSS

## Set Up

**Terminal**

```
npm install -D tailwindcss@3 postcss autoprefixer
```

```
npx tailwindcss init -p
```

```
npm install -D prettier prettier-plugin-tailwindcss --legacy-peer-deps
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
---

**index.css**

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
---

create **prettier.config.cjs** 

```
module.exports = {
  plugins: ["prettier-plugin-tailwindcss"],
  singleQuote: true,
};
```
---
