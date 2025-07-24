# Universal HTML Components

## Overview

**Universal HTML Components** is a monorepo of ultra-lightweight, framework-agnostic wrappers around every standard HTML element. It provides you with a consistent, TypeScript-typed API in **React**, **Vue**, **Angular**, or any other UI framework—even plain JavaScript—so you can:

- **Write once, use anywhere**  
  Each element is exposed as a self-contained package (e.g. `@you/html-components/react`, `@you/html-components/vue`, `@you/html-components/angular`), all following the same API surface and naming conventions.

- **Stay close to the DOM**  
  These components are thin shims over native tags, so you never give up HTML semantics or performance. You get full control over attributes, events, and accessibility—plus optional “polymorphic” support via an `as` prop.

- **Gain uniform tooling & types**  
  Shared build, lint, test, and publishing configurations, plus a central `types/` library with:
  - **`CommonComponentProps`** for cross-framework props like `as`, `isClient`, and `isMemoized`
  - **`ElementSpecificPropsConfig`** helpers to enforce valid HTML-only attributes at compile time
  - **Polymorphic typing utilities** so you only get element-specific props when you render that element

- **Scale across frameworks**  
  Future-proof your design system: add new targets (Svelte, Ember, etc.) by dropping in a new sub-package that follows the same conventions.

### Why “universal-html-components”?

- **Framework independence**  
  Your team can adopt or incrementally migrate to different UI stacks without rewriting all your basic building blocks.
- **Semantic fidelity**  
  No “magic” or proprietary abstractions—these components output real HTML tags, attributes, and ARIA roles.
- **Consistent developer experience**  
  One familiar API across React’s JSX, Vue’s SFC, Angular’s templates, or hyperscript.
- **Zero runtime overhead**  
  No styling, no theming, no CSS-in-JS—just a minimal runtime that forwards props and refs to native elements.

---

*Next up in the README:*
1. **Getting Started** (installation & basic usage examples)  
2. **API Reference** (list of supported elements & shared props)  
3. **Monorepo Structure** (how React, Vue, Angular packages are organized)  
4. **Contributing & Roadmap** (adding new elements or framework targets)
