# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

Learn more about IDE Support for Vue in the [Vue Docs Scaling up Guide](https://vuejs.org/guide/scaling-up/tooling.html#ide-support).



 Tailwind CSS Setup

Install Tailwind CSS and dependencies

 install -D tailwindcss postcss autoprefixer


 Create config files

Create `tailwind.config.js` at the project root:
js
/** @type {import('tailwindcss').Config} */
export default {
	content: [
		"./index.html",
		"./src/**/*.{vue,js}"
	],
	theme: {
		extend: {},
	},
	plugins: [],
}


Create postcss.config.js at the project root:
js
export default {
	plugins: {
		tailwindcss: {},
		autoprefixer: {},
	},
}


 Add Tailwind to your CSS

Create or edit `src/assets/main.css`:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

 Import Tailwind in your main.js

Edit `src/main.js`:
js
import './assets/main.css'


 Run your project


npm run dev




You are now ready to use Tailwind CSS in your Vue components!
