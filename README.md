This is a Next.js template with Typescript, TailwindCSS, and next/font configured

To get started, run:
```bash
pnpm i
pnpx tailwindcss init -p
pnpm dev
```

then copy the following into tailwind.config.js
```js
const { fontFamily } = require('tailwindcss/defaultTheme');

/** @type {import('tailwindcss').Config} */

module.exports = {
  content: ['./src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {
      fontFamily: {
        sans: ['var(--font-inter)', ...fontFamily.sans],
      },
    },
  },
  plugins: [],
};
```