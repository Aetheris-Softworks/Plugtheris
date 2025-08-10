# 🌌 Plugtheris
**The Aetheris Enhancement Project**

![License](https://img.shields.io/github/license/unixetp/Plugtheris?style=for-the-badge&color=green)
![Stars](https://img.shields.io/github/stars/unixetp/Plugtheris?style=for-the-badge&color=yellow)
![Forks](https://img.shields.io/github/forks/unixetp/Plugtheris?style=for-the-badge&color=orange)
![Last commit](https://img.shields.io/github/last-commit/unixetp/Plugtheris?style=for-the-badge&color=informational)
![Open Issues](https://img.shields.io/github/issues/unixetp/Plugtheris?style=for-the-badge&color=critical)



![Plugtheris Banner](images/banner.png)

Plugtheris is an open-source patcher for [Aetheris](#), enabling plugins, custom CSS, and enhanced functionality for Aetheris.  
Inspired by projects like Vencord and BetterDiscord, but built specifically for Aetheris.  

---

## ✨ Features
- 🔌 **Plugins** — easily enable and disable extensions.
- 🎨 **Custom CSS** — style the interface your way.
- ⚡ **Real-time Loading** — changes apply instantly.
- 🌍 **Open Source** — community-driven and collaborative.

---

## 📥 Installation
1. Download the latest version from [Releases](#).
2. Run the installer.
3. Select your Aetheris installation folder.
4. Done.    extends: [
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
