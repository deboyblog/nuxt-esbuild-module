  # Nuxt ESBuild module

Enables [`esbuild-loader`](https://github.com/egoist/esbuild-loader) 
to transpile **JavaScript** and **TypeScript** in Nuxt.

**This is for speeding up development-only**.

When building for production, original Babel settings are used.

## Install

```sh
npm i nuxt-esbuild --save
```

In `nuxt.config.js`:

```js
modules: [
  'nuxt-esbuild'
]
```

## Enabling TypeScript

In `nuxt.config.js`:

```js
modules: [
  'nuxt-esbuild'
],
esbuild: {
  loader: 'ts',
  // Seems to work alright without tsconfig.json though
  tsconfig: 'path-to-tsconfig.json',
},
```

## Notice

This is entirely experimental, no guarantees it will work for everyone.

Follow the [esbuild project](https://github.com/evanw/esbuild) for latest info on its reliability and options.
