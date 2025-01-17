
## Svelte

* **Overview:** Introduces Svelte and its compiler-based approach to building user interfaces.
* **Getting Started:** Guides setting up a Svelte project, preferably using SvelteKit.  Provides alternative setups using Vite, Rollup, and Webpack.  Also mentions editor tooling and community support.
* **.svelte files:** Details the structure of Svelte component files, including `<script>`, `<script module>`, and `<style>` tags.
* **.svelte.js and .svelte.ts files:** Explains how these files enable reusable reactive logic and shared state.
* **Public API of a component:** Describes how to define and use props, reactive variables, and component exports.  Covers topics like fallback values, prop renaming, rest props, updating props, and type safety.
* **Reactivity fundamentals:** Introduces runes, Svelte's reactivity primitives.
* **Runes:** In-depth explanation of runes, including `$state`, `$derived`, `$effect`, `$props`, `$bindable`, `$inspect`, `$host`.  Explains how runes control reactivity, dependencies, and update propagation.  Includes examples and best practices.
* **Basic markup:** Describes HTML enhancements in Svelte, covering tags, element attributes, component props, event handling, text expressions, comments, and HTML injection with `{@html}`.
* **Control flow:**  Explains conditional rendering with `{#if}`, iteration with `{#each}`, asynchronous handling with `{#await}`, and keyed each blocks.  Covers key expressions, destructuring, rest patterns, and else blocks.
* **Data fetching:**  Shows how to fetch data in Svelte, including using the `{#await}` block and integrating with SvelteKit loaders.
* **Scoped styles:**  Details Svelte's component-level CSS scoping mechanism, including specificity and keyframes.
* **Global styles:**  Explains how to apply styles globally using the `:global(...)` modifier and `:global` blocks.
* **Custom properties:**  Demonstrates passing and using CSS custom properties between components.
* **Nested `<style>` elements:**  Clarifies the behavior of nested `<style>` tags.
* **`<svelte:boundary>`:**  Explains error boundaries and how to handle errors within components.
* **`<svelte:window>`:**  Describes adding event listeners and binding to window properties.
* **`<svelte:document>`:** Describes adding event listeners and binding to document properties.
* **`<svelte:body>`:**  Describes adding event listeners and actions to the `<body>` element.
* **`<svelte:head>`:**  Explains inserting elements into `<head>`.
* **`<svelte:element>`:**  Describes rendering dynamic elements.
* **`<svelte:options>`:**  Explains per-component compiler options.
* **Stores:** Explains the store contract and built-in stores (`writable`, `readable`, `derived`, `get`).  Discusses when to use stores and how they interact with runes.
* **Context:**  Details the `getContext`, `setContext`, `hasContext`, and `getAllContexts` functions for managing component context.
* **Lifecycle hooks:**  Covers `onMount`, `onDestroy`, `tick`, and the deprecated `beforeUpdate` and `afterUpdate`.
* **Imperative component API:**  Explains `mount`, `unmount`, `render`, and `hydrate` functions for component instantiation and manipulation.
* **Testing:**  Provides guidance on testing Svelte apps using Vitest and Playwright. Includes examples of unit testing, integration testing, and component testing.
* **TypeScript:**  Explains how to use TypeScript with Svelte, including preprocessor setup, typing props and state, and using the `Component` type.
* **Custom elements:**  Details compiling Svelte components as custom elements, including component lifecycle, options, and limitations.
* **Svelte 4 migration guide:** Instructions for migrating from Svelte 3 to 4.
* **Svelte 5 migration guide:**  Instructions for migrating from Svelte 4 to 5, including reactivity changes, event changes, snippets vs. slots, component instantiation, and other breaking changes.
* **Frequently asked questions (FAQ):** Answers common questions about Svelte usage, tooling, integrations, and more.


## SvelteKit

* **Introduction:** Provides an overview of SvelteKit and its purpose.
* **Creating a project:** Guides setting up a new project using `npx sv create`.
* **Project structure:**  Describes the typical file and directory structure of a SvelteKit project.
* **Web standards:**  Highlights the use of web standards like Fetch API, Stream API, URL API, and Web Crypto.
* **Routing:** Explains SvelteKit's filesystem-based router, including route files (`+page`, `+error`, `+layout`, `+server`), dynamic parameters, and content negotiation. Also covers how types are generated for routes.
* **Loading data:**  Details how to fetch data for pages and layouts using `load` functions, including server-side loads, handling errors and redirects, and streaming with promises.
* **Form actions:**  Explains handling form submissions, including default and named actions, validation, progressive enhancement with `use:enhance`, and handling redirects.
* **Page options:** Describes controlling page rendering with options like `prerender`, `ssr`, `csr`, `trailingSlash`, and `config`.
* **State management:**  Provides guidance on managing state in a server-rendered context, including avoiding shared state on the server, using context for state and stores, and preserving component state during navigation.
* **Building your app:**  Explains the build process, including prerendering and adapting the output for different platforms.
* **Adapters:**  Describes the role of adapters in deploying to various environments and lists official adapters.
* **Zero-config deployments:** Explains using `adapter-auto` for simplified deployments.
* **Node servers:**  Details deploying SvelteKit apps to Node.js servers, including environment variables, options, graceful shutdown, and custom servers.
* **Static site generation:**  Explains using `adapter-static` for SSG.
* **Single-page apps:**  Describes turning a SvelteKit app into an SPA.
* **Cloudflare Pages:**  Details deploying to Cloudflare Pages.
* **Cloudflare Workers:**  Details deploying to Cloudflare Workers.
* **Netlify:**  Details deploying to Netlify.
* **Vercel:**  Details deploying to Vercel.
* **Writing adapters:**  Provides guidance for creating custom adapters.
* **Advanced routing:**  Covers rest parameters, optional parameters, matching, sorting, and encoding routes.
* **Hooks:**  Explains using hooks for server-side and client-side logic, including `handle`, `handleFetch`, `handleError`, `locals`, `init`, `reroute`, and `transport`.
* **Errors:**  Describes handling expected and unexpected errors, including responses and type safety.
* **Link options:**  Explains customizing link behavior with attributes like `data-sveltekit-preload-data`, `data-sveltekit-preload-code`, and others.
* **Service workers:**  Details using service workers for offline support and precaching.
* **Server-only modules:**  Explains creating modules that only run on the server.
* **Snapshots:**  Describes capturing and restoring ephemeral DOM state.
* **Shallow routing:**  Explains creating history entries without navigation.
* **Packaging:** Explains how to package Svelte libraries using `@sveltejs/package`.
* **Auth:** Provides high-level guidance on implementing authentication and authorization in SvelteKit.
* **Performance:**  Offers tips for optimizing SvelteKit app performance, including diagnosing issues, optimizing assets, and improving navigation.
* **Images:**  Details optimizing images using Vite, `@sveltejs/enhanced-img`, and CDNs.
* **Accessibility:**  Explains SvelteKit's accessibility features and provides guidance for building accessible apps.
* **SEO:**  Covers SEO best practices for SvelteKit apps.
* **Frequently asked questions (FAQ):**  Answers common questions about SvelteKit usage, integrations, and deployment.
* **Glossary:** Defines key terms related to SvelteKit's rendering and routing.
* **Additional resources:**  Links to examples, community support, and migration guides.


## Svelte CLI

* **Overview:**  Introduces the Svelte CLI (`sv`).
* **`sv create`:** Explains creating new SvelteKit projects.
* **`sv add`:** Explains adding features and integrations to existing projects.
* **`sv check`:**  Explains checking for errors and warnings in projects.
* **`sv migrate`:** Explains migrating Svelte and SvelteKit codebases.


