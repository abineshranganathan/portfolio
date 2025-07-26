# Selected designs
- [Portfolio 1](https://www.figma.com/design/J7lkY29aGHdusNAmcE7tAF/Portfolio--Community-?node-id=0-1&p=f&t=KyYCQLXle0cpRcqT-0)
- [Portfolio 2](https://www.figma.com/design/SYUJKJntUA0i8Wdxej726n/Portfolio-Design--Community-?node-id=0-1&p=f&t=BfWGmnsBrkIBOVMw-0)
- [Portfolio 3](https://www.figma.com/design/bVU3lqrnc5msToYNgFRT8L/Personal-Portfolio---Porrtfolio-App--Community-?node-id=0-1&p=f&t=dE3KJXzPD07JnmNZ-0)

# Reference UI
- [Repo](https://github.com/emmabostian/developer-portfolios)
  - [Tajmirul](https://www.me.toinfinite.dev/)

# "DevConnect" – A Developer Portfolio & Community Hub
This project can demonstrate:
- React (hooks, context, components)
- Tailwind CSS or styled-components
- Responsive design
- API integration (REST or GraphQL)
- State management (Context API, Redux Toolkit or Zustand)
- Routing (React Router)
- Form validation (React Hook Form + Yup)
- Animations (Framer Motion)
- Accessibility and semantic HTML
- Code splitting & lazy loading
- Unit testing (Jest + React Testing Library)

# 🧩 Project Features:
1. Home Page
  - Beautiful hero section
  - Animated intro with scroll effects

2. Developer Profile Page
  - CRUD for education, experience, skills
  - Avatar upload
  - GitHub integration to fetch pinned repos

3. Community Feed
  - Posts with like/comment system
  - Markdown support for posts
  - Search and filter posts
  - Infinite scroll or pagination

4. Dashboard (Authenticated Area)
  - User login/signup (Firebase/Auth0)
  - JWT/token-based auth
  - Settings & theme toggle (dark/light)

5. Admin Panel (Optional)
  - Approve or delete posts
  - See all users

🌐 Tech Stack:
- Frontend: React + Vite/CRA + Tailwind
- State Management: Redux Toolkit or Context API
- Backend (optional): Firebase / Node.js + Express
- Database (optional): Firestore / MongoDB
- CI/CD: GitHub Actions + Netlify/Vercel
- Testing: Jest + Cypress

# 🗂Folder Structure Example
```html
src/
├── components/
├── pages/
├── hooks/
├── services/
├── context/
├── routes/
├── assets/
├── utils/
└── App.jsx
```

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default tseslint.config([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      ...tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      ...tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      ...tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```
