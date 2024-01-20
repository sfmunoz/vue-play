# vue-play

This project is meant to be a playground for [Vue 3](https://vuejs.org/) + [Vite](https://vitejs.dev).

## Init

I chose **No** for every option to have a vanilla environment:

```sh
$ npm create vue@latest
(...)
✔ Project name: … vue-play
✔ Add TypeScript? … No / Yes
✔ Add JSX Support? … No / Yes
✔ Add Vue Router for Single Page Application development? … No / Yes
✔ Add Pinia for state management? … No / Yes
✔ Add Vitest for Unit Testing? … No / Yes
✔ Add an End-to-End Testing Solution? › No
✔ Add ESLint for code quality? … No / Yes
(...)
```

I'm using the following **npm/node** versions:

```sh
$ npm version
(...)
  npm: '10.2.4',
  node: '21.5.0',
(...)
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

This is the result of a **vite build** execution within **vue-play** project folder:

```sh
$ rm -rf dist

$ vite build
vite v5.0.12 building for production...
✓ 23 modules transformed.
dist/index.html                  0.43 kB │ gzip:  0.28 kB
dist/assets/index-WjEyzLJD.css   3.71 kB │ gzip:  1.19 kB
dist/assets/index-avtuWnnn.js   63.15 kB │ gzip: 25.00 kB
✓ built in 1.19s

$ find dist/ -type f -printf '%h/%f: %s bytes\n' | sort
dist/assets/index-avtuWnnn.js: 63158 bytes
dist/assets/index-WjEyzLJD.css: 3706 bytes
dist/favicon.ico: 4286 bytes
dist/index.html: 430 bytes
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

Links rendered by the project itself are useful:

* **Documentation**: Vue’s [official documentation](https://vuejs.org/) provides you with all information you need to get started.
* **Tooling**: This project is served and bundled with [Vite](https://vitejs.dev/guide/features.html). The recommended IDE setup is [VSCode](https://code.visualstudio.com/) + [Volar](https://github.com/johnsoncodehk/volar). If you need to test your components and web pages, check out [Cypress](https://www.cypress.io/) and [Cypress Component Testing](https://on.cypress.io/component). More instructions are available in README.md.
* **Ecosystem**: Get official tools and libraries for your project: [Pinia](https://pinia.vuejs.org/), [Vue Router](https://router.vuejs.org/), [Vue Test Utils](https://test-utils.vuejs.org/), and [Vue Dev Tools](https://github.com/vuejs/devtools). If you need more resources, we suggest paying [Awesome Vue](https://github.com/vuejs/awesome-vue) a visit.
* **Community**: Got stuck? Ask your question on [Vue Land](https://chat.vuejs.org/), our official Discord server, or [StackOverflow](https://stackoverflow.com/questions/tagged/vue.js). You should also subscribe to [our mailing list](https://news.vuejs.org/) and follow the official [@vuejs](https://twitter.com/vuejs) twitter account for latest news in the Vue world.
* **Support Vue**: As an independent project, Vue relies on community backing for its sustainability. You can help us by [becoming a sponsor](https://vuejs.org/sponsor/).
