# [astro-query] 🗜️

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

To install `astro-query`, run the following from your project directory and
follow the prompts:

Using NPM:

```sh
npx astro add astro-query
```

Using Yarn:

```sh
yarn astro add astro-query
```

Using PNPM:

```sh
pnpx astro add astro-query
```

### Install dependencies manually

First, install the `astro-query` integration like so:

```
npm install -D -E astro-query
```

Then, apply this integration to your `astro.config.*` file using the
`integrations` property:

**`astro.config.ts`**

```ts
import query from "astro-query";

export default { integrations: [query()] };
```

## Getting started

#### Set `Logger` to `0` if you do not want to see debug messages. Default is `2`.

**`astro.config.ts`**

```ts
import query from "astro-query";

export default {
	integrations: [
		query({
			Logger: 0,
		}),
	],
};
```

[astro-query]: https://npmjs.org/astro-query
[astro-integration]: https://docs.astro.build/en/guides/integrations-guide/

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for a history of changes to this integration.

[![Lightrix logo](https://raw.githubusercontent.com/Lightrix/NPM/main/.github/Image/favicon.png "Built with Lightrix/NPM")](https://github.com/Lightrix/NPM)
<sup>Built with [`Lightrix/NPM`](https://github.com/Lightrix/NPM).</sup>
