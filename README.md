# Chrome Extension V3 Boilerplate

> Very basic [Webpack](https://webpack.js.org/) boilerplate for developing Chrome Extension compatible with [manifest V3](https://developer.chrome.com/docs/extensions/mv3/intro/).

## Features

- [TypeScript](https://www.typescriptlang.org/) support
- [CSS Modules](https://github.com/css-modules/css-modules) support
- Auto-build with Webpack in dev mode (no browser hot reload, though)
- Clean, straightforward and ready-to-use [project structure](#project-structure)

## Getting started

[Node.js](https://nodejs.org/en/) is requierd.

1. Clone this repository
2. Run `npm install` command in the project directory
3. Configure _src/manifest.json_ and _package.json_ files to your will
4. Run `npm run dev` or `npm run build` in the project directory (it will generate _build_ directory)
5. In your Chrome Browser:
   1. Go to <chrome://extensions/>
   2. Turn on **Developer mode**
   3. Click **Load unpacked**
   4. Select the _build_ directory
   5. Your extension should appear in Chrome

## Project structure

```
📦chrome-extension-v3-boilerplate
 ┣ 📂src
 ┃ ┣ 📂css
 ┃ ┃ ┣ 📂modules
 ┃ ┃ ┃ ┗ name.module.css
 ┃ ┃ ┣ 📜content.css
 ┃ ┃ ┣ 📜options.css
 ┃ ┃ ┗ 📜popup.css
 ┃ ┣ 📂html
 ┃ ┃ ┣ 📜content.html
 ┃ ┃ ┣ 📜options.html
 ┃ ┃ ┗ 📜popup.html
 ┃ ┣ 📂img
 ┃ ┃ ┗ 📜example.png
 ┃ ┣ 📂ts
 ┃ ┃ ┣ 📜background.ts
 ┃ ┃ ┣ 📜content.ts
 ┃ ┃ ┣ 📜options.ts
 ┃ ┃ ┗ 📜popup.ts
 ┃ ┗ 📜manifest.json
 ┣ 📜.gitignore
 ┣ 📜declaration.d.ts
 ┣ 📜package.json
 ┣ 📜README.md
 ┣ 📜tsconfig.json
 ┗ 📜webpack.config.js
```

Notes:

- _manifest.json_ should be in _src_ directory
- All script files should be in _src/ts_, however you can create subdirectories for module scripts
- All HTML files should be in _src/html_ directory
- CSS Modules files should be named as `*.module.css`, but they don't have to be placed in _src/css/modules_ directory
- You can setup your TypeScript preferences in _tsconfig.json_ file

## Notes

This simple boilerplate was created for my personal extension development. It was heavily inspired by [chrome-extension-webpack-boilerplate](https://github.com/samuelsimoes/chrome-extension-webpack-boilerplate) project. I believe that for someone it might be a good starting point.

## Contact

Created by [@michaltkacz](https://github.com/michaltkacz) - feel free to contact me!
