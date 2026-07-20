<div align="center">

<img src="https://webisters.github.io/docs/assets/logo.svg" alt="Webisters" width="96" height="96">

# Webisters

**A modern, lightweight full-stack PHP framework — batteries-included libraries and ready-to-run project templates.**

[![Docs](https://img.shields.io/badge/docs-docs.webisters.com-0052ff?style=flat-square&logo=readthedocs&logoColor=white)](https://docs.webisters.com)
[![Website](https://img.shields.io/badge/web-webisters.com-111111?style=flat-square&logo=googlechrome&logoColor=white)](https://webisters.com)
[![PHP](https://img.shields.io/badge/PHP-%3E%3D8.2-777bb4?style=flat-square&logo=php&logoColor=white)](https://www.php.net/)
[![Composer](https://img.shields.io/badge/Composer-2.x-885630?style=flat-square&logo=composer&logoColor=white)](https://getcomposer.org/)
[![License](https://img.shields.io/badge/license-MIT-3fb950?style=flat-square)](https://github.com/webisters/webisters/blob/main/LICENSE)

[**📖 Documentation**](https://docs.webisters.com) · [Get Started](#-get-started) · [Libraries](#-libraries) · [Project Templates](#-project-templates)

</div>

---

## What is Webisters?

Webisters is a full-stack PHP framework (PHP `>=8.2`) built as a **monorepo of independently-versioned Composer packages**. Take the whole framework, or compose your app from just the libraries you need — every package lives under the `Framework\*` namespace and installs through Composer.

- 🧩 **Modular** — 29 focused libraries (routing, database, http, session, validation, …) that work together or standalone.
- ⚡ **Lightweight** — minimal dependencies, fast boot, no heavy runtime.
- 🔋 **Batteries included** — MVC, CLI tooling, migrations, caching, crypto, i18n, logging, and more.
- 🚀 **Scaffold in seconds** — generate app / API / single-file / static-site projects with one command.

## 🚀 Get Started

```bash
# 1. Install the global CLI
composer global require webisters/webisters

# 2. Create a project
webisters new-app my-app     # full MVC application
webisters new-api my-api     # REST API
webisters new-one my-one     # single-file style app
webisters new-site my-site   # static site
```

> [!IMPORTANT]
> Enable the required PHP extensions first — `intl`, `sodium`, `gd`, `mysqli`, `curl`, `fileinfo`, `json`, `simplexml`, `dom`, `libxml`, plus `openssl` and `zip` for Composer. See the [**Requirements guide**](https://docs.webisters.com/guides/webisters/#requirements).

📖 **Full documentation lives at [docs.webisters.com](https://docs.webisters.com)** — guides, per-library references, and full API docs generated from source.

## 📚 Libraries

| Library | What it does |
| --- | --- |
| [autoload](https://github.com/webisters/autoload) | PSR-4 class autoloader, file locator, and opcache preloader |
| [cache](https://github.com/webisters/cache) | Caching with APCu, Redis, Memcached, and filesystem drivers |
| [cli](https://github.com/webisters/cli) | Framework for building command-line apps |
| [coding-standard](https://github.com/webisters/coding-standard) | Shared PHP-CS-Fixer configuration and style |
| [config](https://github.com/webisters/config) | Config loader for PHP, INI, JSON, XML, YAML, ENV, and DB sources |
| [crypto](https://github.com/webisters/crypto) | libsodium cryptography: boxes, signing, hashing, passwords |
| [database](https://github.com/webisters/database) | MySQLi layer with a fluent query builder and prepared statements |
| [database-extra](https://github.com/webisters/database-extra) | Database migrations and seeders |
| [date](https://github.com/webisters/date) | Immutable, locale-aware date/time built on ext-intl |
| [debug](https://github.com/webisters/debug) | Exception handler, timers, collectors, and a debug bar |
| [dev-commands](https://github.com/webisters/dev-commands) | Console commands for migrations, seeding, routing, schema |
| [email](https://github.com/webisters/email) | Email composition and sending (headers, priorities, MIME) |
| [events](https://github.com/webisters/events) | Lightweight event dispatcher |
| [factories](https://github.com/webisters/factories) | Lazy creation and caching of named service instances |
| [front](https://github.com/webisters/front) | Front-end asset tooling: SASS compilation and view building |
| [helpers](https://github.com/webisters/helpers) | Utilities incl. dot-notation array access and isolation |
| [http](https://github.com/webisters/http) | HTTP messages: requests, responses, cookies, CSRF, CSP |
| [http-client](https://github.com/webisters/http-client) | cURL-based HTTP client |
| [image](https://github.com/webisters/image) | Image manipulation (resize, crop, convert) on GD |
| [language](https://github.com/webisters/language) | i18n and translation with locale fallbacks |
| [log](https://github.com/webisters/log) | Logging with file, syslog, email, and SAPI handlers |
| [minify](https://github.com/webisters/minify) | Minifier for CSS, JavaScript, and HTML |
| [mvc](https://github.com/webisters/mvc) | MVC foundation: App container, controllers, models, views |
| [pagination](https://github.com/webisters/pagination) | Pagination links and metadata for result sets |
| [routing](https://github.com/webisters/routing) | Attribute- and code-based HTTP router |
| [session](https://github.com/webisters/session) | Sessions with files, database, Redis, Memcached handlers |
| [testing](https://github.com/webisters/testing) | PHPUnit base cases and app testing utilities |
| [theme](https://github.com/webisters/theme) | Theme management for view themes |
| [validation](https://github.com/webisters/validation) | Data and file validation with a configurable rule set |

## 🧱 Project Templates

| Template | Use it for |
| --- | --- |
| [app](https://github.com/webisters/app) | Full-stack MVC application |
| [api](https://github.com/webisters/api) | REST API service |
| [one](https://github.com/webisters/one) | Single-file / micro app |
| [site](https://github.com/webisters/site) | Static website |

## 📦 Core Packages

| Package | Description |
| --- | --- |
| [framework](https://github.com/webisters/framework) | Metapackage bundling the core libraries and canonical autoload map |
| [webisters](https://github.com/webisters/webisters) | Global CLI installer that scaffolds new projects |
| [docs](https://github.com/webisters/docs) | Source for **[docs.webisters.com](https://docs.webisters.com)** |

## 👑 Top Contributor

<a href="https://github.com/HafizMMoaz">
  <img src="https://github.com/HafizMMoaz.png" width="80" height="80" style="border-radius:50%" alt="HafizMMoaz">
</a>

**[Hafiz Muhammad Moaz — @HafizMMoaz](https://github.com/HafizMMoaz)** — creator and lead maintainer of the Webisters framework. 🏆

Thanks to everyone who reports issues, improves the docs, and contributes code. Contributions are welcome across every repository.

## 🤝 Contributing & Support

- 📖 **Docs:** [docs.webisters.com](https://docs.webisters.com)
- 🌐 **Website:** [webisters.com](https://webisters.com)
- 🐛 **Issues:** open one in the relevant repository
- 💬 **Forum:** [github.com/webisters/forum](https://github.com/webisters/forum)
- ✉️ **Email:** support@webisters.com

## 📄 License

Webisters is open-source software released under the [MIT License](https://github.com/webisters/webisters/blob/main/LICENSE).

<div align="center">
<sub>Built with ❤️ by the Webisters team · <a href="https://docs.webisters.com">docs.webisters.com</a></sub>
</div>
