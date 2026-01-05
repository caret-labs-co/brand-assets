<!-- Project Header -->
<div align="center">
	<h1 class="projectName">Brand Assets</h1>
	<p class="projectBadges info">
		<img src="https://johng.io/badges/category/Other.svg" alt="Project category" title="Project category">
		<img src="https://img.shields.io/github/repo-size/caret-labs-co/brand-assets.svg" alt="Repository size" title="Repository size">
		<a href="LICENSE"><img src="https://img.shields.io/github/license/caret-labs-co/brand-assets.svg" alt="Project license" title="Project license"/></a>
	</p>
	<p class="projectDesc">
		Logos, icons, and other brand assets for Caret Labs.
	</p>
	<br/>
</div>

## 👋 About

This repository contains the official brand assets for [Caret Labs](https://caretlabs.co). It's intended to be consumed by other Caret Labs projects as a [Git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules).

## 📦 Installation

### As a Git submodule

```sh
git submodule add https://github.com/caret-labs-co/brand-assets.git path/to/brand
git submodule update --init --recursive
```

> [!IMPORTANT]
> If your project uses CI, make sure the checkout step initialises submodules, or the assets won't be available at build time:
>
> ```yaml
> # .github/workflows/ci.yml
> - uses: actions/checkout@v6
>   with:
>     submodules: recursive
> ```

### Keeping assets up to date

To pull the latest assets into a project that already has the submodule:

```sh
git submodule update --remote --merge
```

## 🕹️ Usage

Reference assets by path relative to the submodule root. In a project with the submodule mounted at `src/assets/brand/`:

```html
<img src="src/assets/brand/logo.svg" alt="Caret Labs" />
```

### Referencing assets in a README

GitHub's Markdown renderer doesn't resolve paths into submodule directories. Use a raw URL pointing directly to this repo instead:

```md
![Caret Labs logo](https://raw.githubusercontent.com/caret-labs-co/brand-assets/main/logo.svg)
```

See the [contribution guide](../../contribute) for more details.

## 🧾 License

Copyright © 2026 [Caret Labs](https://caretlabs.co) ([@caret-labs-co](https://github.com/caret-labs-co)).

All rights reserved.

## 🖇️ Related

### In the Wild

Notable projects that depend on this one:

- **👤 [caret-labs-co](https://github.com/caret-labs-co/caret-labs-co)**: Landing page for Caret Labs.
