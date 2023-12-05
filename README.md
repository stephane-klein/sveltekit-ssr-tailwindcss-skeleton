# SvelteKit SSR with TailwindCSS Stéphane Klein skeleton

I try to gather and maintain, in this skeleton, my standard components configuration
that I use in my SvelteKit web application projects.

TailwindCSS has been installed with [Add Tailwind CSS to Svelte](https://github.com/svelte-add/tailwindcss/) ["Svelte
Add"](https://github.com/svelte-add), with this command:

```
$ pnpx svelte-add@latest tailwindcss --tailwindcss-forms --tailwindcss-typography
```

Components and libraries:

- ✅ [SSR](https://kit.svelte.dev/docs/page-options#ssr) [SvelteKit](https://github.com/sveltejs/kit) with [Hydration](https://kit.svelte.dev/docs/glossary#hydration)
- ✅ [TailwindCSS](https://github.com/tailwindlabs/tailwindcss)

Tooling:

- ✅ [asdf](https://asdf-vm.com/)
- ✅ [NodeJS](https://nodejs.org/en/)
- ✅ [pnpm](https://pnpm.io/)
- ✅ [Prettier](https://prettier.io/)
- ✅ [ESlint](https://eslint.org/)

Methods:

- Deployment based by Docker

Not included:

- No TypeScript support

## Getting started

```sh
$ asdf install
```

```sh
$ pnpm install
```

Start database engine:

```sh
$ docker compose up -d --wait
$ ./scripts/init.sh
$ ./scripts/fixtures.sh
```

Start web server:

```sh
$ pnpm run dev
```

Go to http://localhost:5173/

## Database migration

```
$ pnpm run migrate:watch
```

Apply migration in `migrations/current.sql` and commit:

```
$ pnpm run migrate:commit
```

## Prettier

Launch Prettier check:

```sh
$ pnpm run prettier-check
```

Apply Prettier fix example:

```sh
$ pnpm run prettier src/app.html
```

## ESlint

```sh
$ pnpm run eslint
```
