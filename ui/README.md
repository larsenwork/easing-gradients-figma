# Typescript template for Svelte v3

---

# svelte app

This is a project template for [Svelte](https://svelte.dev) apps. It lives at https://github.com/pyoner/svelte-typescript

## Install

### For Linux, MacOs users
```bash
mkdir svelte-app
curl -L https://github.com/pyoner/svelte-typescript/tarball/master > svelte-typescript.tar
tar --strip-components=3 --wildcards --one-top-level=svelte-app -xf svelte-typescript.tar */packages/template
```

### For Windows users
Download https://github.com/pyoner/svelte-typescript/archive/master.zip and extract template from `packages/template`

*Note that you will need to have [Node.js](https://nodejs.org) installed.*


## Get started

Install the dependencies...

```bash
cd svelte-app
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.


## Deploying to the web

### With [now](https://zeit.co/now)

Install `now` if you haven't already:

```bash
npm install -g now
```

Then, from within your project folder:

```bash
now
```

As an alternative, use the [Now desktop client](https://zeit.co/download) and simply drag the unzipped project folder to the taskbar icon.

### With [surge](https://surge.sh/)

Install `surge` if you haven't already:

```bash
npm install -g surge
```

Then, from within your project folder:

```bash
npm run build
surge public
```
