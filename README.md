# vue-play

This project is meant to be a playground for Vue 3 + Vite.

## Project setup

I chose **No** for every option to have a vanilla environment:

```sh
$ npm create vue@latest

✔ Project name: … vue-play
✔ Add TypeScript? … No / Yes
✔ Add JSX Support? … No / Yes
✔ Add Vue Router for Single Page Application development? … No / Yes
✔ Add Pinia for state management? … No / Yes
✔ Add Vitest for Unit Testing? … No / Yes
✔ Add an End-to-End Testing Solution? › No
✔ Add ESLint for code quality? … No / Yes
```

## IDE setup

I'm using the recommended tooling on ([https://vuejs.org/guide/quick-start.html](https://vuejs.org/guide/quick-start.html):

* [VSCode](https://code.visualstudio.com/)
* [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) → don't use Vetur
* [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project setup

```sh
npm install
```

## Management

Tweak **PATH** to use **vite** command:

```sh
export PATH=`pwd`/node_modules/.bin:$PATH
```

### Compile and hot-reload for development

```sh
vite
```

**npm** based alternative*:

```sh
npm run dev
```

### Compile and minify for production

```sh
vite build
```

**npm** based alternative*:

```sh
npm run build
```
