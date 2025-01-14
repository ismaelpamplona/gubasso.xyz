# gubasso.xyz

> Welcome to my personal website!

<!-- toc -->

- [new title](#new-title)
- [create-svelte](#create-svelte)
  - [Creating a project](#creating-a-project)
  - [Developing](#developing)
  - [Building](#building)
- [Prettier](#prettier)
- [Pre-commit](#pre-commit)

<!-- tocstop -->

# new title

# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

# Prettier

```sh
npx prettier --write --plugin prettier-plugin-svelte .
```

As part of your scripts in `package.json`:

```json
"format": "prettier --write  --plugin prettier-plugin-svelte ."
```

# Pre-commit

- Install pre-commit: https://pre-commit.com/
- Run commands for the first time

```sh
pre-commit install
pre-commit run --all-files
```
