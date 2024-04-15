# 👉🏻 [Query.]

This **[Astro integration][astro-integration]** allows you to use SQL queries
inside your components using PRQL.

## Installation

There are two ways to add integrations to your project. Let's try the most
convenient option first!

### `astro add` command

Astro includes a CLI tool for adding first party integrations: `astro add`. This
command will:

1. (Optionally) Install all necessary dependencies and peer dependencies
2. (Also optionally) Update your `astro.config.*` file to apply this integration

To install `@playform/query`, run the following from your project directory and
follow the prompts:

Using NPM:

```sh
npx astro add @playform/query
```

Using Yarn:

```sh
yarn astro add @playform/query
```

Using PNPM:

```sh
pnpx astro add @playform/query
```

### Install dependencies manually

First, install the `@playform/query` integration like so:

```sh
npm install -D -E @playform/query
```

Then, apply this integration to your `astro.config.*` file using the
`integrations` property:

**`astro.config.ts`**

```ts
import query from "@playform/query";

export default { integrations: [query()] };
```

## Getting started

#### Set `Logger` to `0` if you do not want to see debug messages. Default is `2`.

**`astro.config.ts`**

```ts
import query from "@playform/query";

export default {
	integrations: [
		query({
			Logger: 0,
		}),
	],
};
```

[Query]: https://npmjs.org/@playform/query
[astro-integration]: https://docs.astro.build/en/guides/integrations-guide/

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for a history of changes to this integration.
