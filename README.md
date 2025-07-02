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
---

### 📏Spacing

####  Padding (p- = all sides, px- = x-axis, py- = y-axis)
```
p-0    p-2    p-4    px-4    py-2    pl-6    pr-8
```

#### Margin (m- = all sides, mx- = x-axis, my- = y-axis)
```
m-0    m-2    m-4    mx-4    my-2    ml-6    mr-8
```
---

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
---

### 📐 Display & Layout

#### Display
```
block     inline-block     inline  
flex      inline-flex      grid     hidden
```

#### Flexbox Helpers
```
flex-row      flex-col       flex-wrap  
items-center  justify-between  gap-4
```

#### Grid Helpers
```
grid-cols-1   grid-cols-2   grid-cols-3  
col-span-1    col-span-2    gap-4
```
---

### 📱Responsive Design & Breakpoints

**🧠 What is a Breakpoint?**

- A breakpoint in responsive design defines the screen width at which the layout or style should adapt. It allows your design to respond to different devices like mobile phones, tablets, and desktops.


- 📏 Default Tailwind Breakpoints

Tailwind CSS uses **min-width** breakpoints by default:

| Breakpoint | Min Width | Common Devices        |
|------------|-----------|------------------------|
| `sm`       | 640px     | Small screens (phones) |
| `md`       | 768px     | Medium screens (tablets) |
| `lg`       | 1024px    | Large screens (laptops) |
| `xl`       | 1280px    | Extra large screens (desktops) |
| `2xl`      | 1536px    | Ultra-wide screens (TVs, large monitors) |


```
<p class="text-sm md:text-lg lg:text-xl">
  Responsive font size based on screen width
</p>
```
---
