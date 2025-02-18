# Vite React Electron

How to use Vite to build a React application that runs in Electron

## Requirements

- Node.js
- npm

## Create Vite application

Use Vite to create a React app, then install.

```shell
npm create vite@latest .
npm install
```

## Install Electron

Install electron, then create `main.cjs`

```shell
npm install electron --save-dev
```

## Update `package.json`

Add `electron` script

```json
"scripts": {
  ...
  "electron": "electron main.cjs"
}
```

## Add main to `package.json`

```json
  "name": "vite-react-electron",
  ...
  "main": "main.cjs",
  ...
```

## Update `vvite.config.js`

```javascript
  base: "./",
  build: {
    outDir: "dist",
  },
```

## Build

Build the React app

```shell
npm run build
```

## Run Electron

```shell
npm run electron
```
