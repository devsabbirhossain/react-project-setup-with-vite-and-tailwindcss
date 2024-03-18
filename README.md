# React project setup with vite and tailwindcss
A complete guid how to create a react project using vite and tailwindcss 

```
npm create vite@latest <project-name> -- --template react
```

Now go to the project directory

```
cd <project-name>
```

Install Tailwindcss to your project

```
npm install -D tailwindcss postcss autoprefixer
```
Add Tailwindcss config file to your project

```
npx tailwindcss init -p
```
update tailwindcss config file with these code to apply tailwindcss 

```
/** @type {import('tailwindcss').Config} */
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```
Import tailwindcss css to your stylesheet file

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
