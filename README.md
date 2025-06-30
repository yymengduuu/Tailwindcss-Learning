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

## common Tailwind CSS utility classes

### 🎨Color

#### Text Color
```
text-black    text-white    text-gray-500  
text-red-500  text-green-500  text-blue-500
```

#### Background Color
```
bg-white    bg-black    bg-gray-100  
bg-red-100  bg-green-200  bg-blue-300
```

#### Border Color
```
border-black  border-white  border-gray-300  
border-red-400  border-green-400  border-blue-400
```

### 📏Spacing

####  Padding (p- = all sides, px- = x-axis, py- = y-axis)
```
p-0    p-2    p-4    px-4    py-2    pl-6    pr-8
```

#### Margin (m- = all sides, mx- = x-axis, my- = y-axis)
```
m-0    m-2    m-4    mx-4    my-2    ml-6    mr-8
```

### 🔲 Borders

#### Border Width
```
border       // default = 1px
border-2     border-4     border-8
```

#### Border Radius
```
rounded      rounded-sm   rounded-md  
rounded-lg   rounded-xl   rounded-full
```

#### Border Style
```
border-solid  border-dashed  border-dotted  border-none
```
