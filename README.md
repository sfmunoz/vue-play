# vue-play

This project is meant to be a playground for Vue 3 + Vite.

## Init

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

## Setup

```sh
$ npm install
```

## Management

Tweak **PATH** to use **vite** command:

```sh
$ export PATH=`pwd`/node_modules/.bin:$PATH
```

Useful commands can be figured out using **package.json** details:

```sh
$ jq .scripts < package.json
{
  "dev": "vite",
  "build": "vite build",
  "preview": "vite preview"
}
```

### Compile and hot-reload for development

```sh
$ vite
```

**npm** based alternative:

```sh
$ npm run dev
```

### Compile and minify for production

```sh
$ vite build
```

**npm** based alternative:

```sh
$ npm run build
```

## Links

* IDE setup ([https://vuejs.org/guide/quick-start.html](https://vuejs.org/guide/quick-start.html) recommended tooling):
  * [VSCode](https://code.visualstudio.com/)
  * [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) → Vetur shouldn't be used
  * [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)
* [Vue.js](https://vuejs.org/):
  * [Vue.js Introduction](https://vuejs.org/guide/introduction.html)
  * [Vue.js Quick Start](https://vuejs.org/guide/quick-start)
* [https://vitejs.dev](Vite):
  * **[Vite Configuration](https://vitejs.dev/config/)** → customize project config
  * [Vite guide](https://vitejs.dev/guide/)
