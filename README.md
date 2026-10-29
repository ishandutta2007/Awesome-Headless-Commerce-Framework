# Awesome-Headless-Commerce-Framework

# Top Headless Commerce Framework Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Composable Storefronts, API-First Commerce & Framework-Agnostic Toolkits*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Headless Commerce Frameworks**. These tools enable developers to decouple the frontend presentation layer from backend commerce logic—building fast, customizable storefronts that consume product, cart, and checkout data via APIs from platforms like Shopify, Medusa, Saleor, or custom backends.

**Examples** include Hydrogen, Next.js, Nuxt.js, Gatsby, Remix, Astro, SvelteKit, Angular Universal, SolidStart, and Frontity (the category leaders).

**Open-source emphasis**: Headless Commerce is a domain where open-source tooling is **exceptionally mature and production-proven**—but the "framework" landscape is shifting. **Hydrogen** is no longer a framework itself; as of October 2026 it is a **framework-agnostic library** you add to React Router, Next.js, or any JavaScript stack, handling cart, variants, pricing, and analytics while your framework owns routing and rendering . **Next.js Commerce** provides Vercel's official Shopify starter using React Server Components and App Router . **Frontity** remains a dedicated React framework specifically for headless WordPress . **Svelte Commerce** offers multi-platform connectors spanning 20+ commerce backends . **Astro** provides a content-optimized storefront template with zero JavaScript by default . The critical caveat: most "frameworks" here are **general-purpose web frameworks** adapted for commerce, not commerce-specific frameworks—and Hydrogen's pivot to a library means the era of commerce-specific frontend frameworks is consolidating toward framework-agnostic toolkits.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Shopify Hydrogen](https://hydrogen.shopify.dev/)**  
  Shopify's commerce toolkit, now a **framework-agnostic library** (October 2026) rather than a framework; add it to React Router, Next.js, or any JS stack to get cart, variants, pricing, Shop Pay, and analytics . Hosting on Oxygen remains free, but you can deploy anywhere (Vercel, Cloudflare Workers, Node, Deno) .

- **[Vercel (Next.js Commerce)](https://vercel.com/)**  
  Vercel maintains the Next.js Commerce starter, actively supporting a Shopify version with React Server Components and App Router; other commerce providers can fork and swap the Shopify implementation .

- **[Netlify](https://www.netlify.com/)**  
  Hosting platform commonly paired with Gatsby, Astro, and other headless frameworks; provides Git-based deployments and serverless functions.

- **[Cloudflare Pages](https://pages.cloudflare.com/)**  
  Edge hosting for headless storefronts with Workers integration; supports frameworks like Astro, Next.js, and SvelteKit.

- **[Oxygen (Shopify)](https://shopify.dev/docs/api/hydrogen/latest/oxygen)**  
  Shopify's hosting platform for Hydrogen storefronts; free and optimized for Shopify commerce APIs, but no longer required for Hydrogen usage .

## Open-Source GitHub Projects

### Framework-Agnostic Commerce Toolkits

- **[Hydrogen (Shopify)](https://github.com/Shopify/hydrogen)**  
  The pivot from framework to **library** is the defining shift of 2026. Hydrogen now handles commerce primitives—cart state, variant selection, buyer-currency pricing, analytics, Shop Pay, customer login—while your chosen framework (React Router, Next.js, Vue, or any fetch-capable runtime) owns routing and rendering . Ships with **20 agent skills** that teach coding agents how to wire storefronts, versioned to your installed package. Host anywhere, including Oxygen (free). **The most strategically important open-source commerce toolkit** for Shopify-based headless builds, precisely because it no longer forces a framework choice.

### Commerce-Specific Frameworks & Starters

- **[Next.js Commerce](https://github.com/vercel/commerce)**  
  Vercel's official high-performance storefront using **React Server Components, Server Actions, Suspense, and useOptimistic** . Actively maintained for Shopify; other providers fork and swap `lib/shopify`. **The reference implementation for Next.js App Router commerce**—not a general framework, but the starter that defines modern React commerce patterns.

- **[Frontity](https://github.com/frontity/frontity)**  
  React-based framework specifically for **headless WordPress** storefronts and blogs . Connects to WordPress REST API; runs on Node.js separate from the WordPress server. **The dedicated framework for WordPress-backed headless sites**—not general commerce, but the only framework with native WordPress integration as its core design goal.

- **[Svelte Commerce](https://github.com/itswadesh/svelte-commerce)**  
  Multi-platform headless commerce frontend with **connectors for 20+ backends** including Vendure, Medusa, Saleor, Shopware, WooCommerce, Magento, Spree, and commercetools . Coverage varies by platform (Litekart and Vendure at 39/43 endpoints; Bagisto at 22/43). **The broadest backend-agnostic commerce frontend**, though connector maturity is uneven and none have been tested against live production instances.

- **[Astro Audiophile (Azion)](https://github.com/aziontech/astro-audiophile)**  
  Astro-based ecommerce template with product listings, detail pages, cart, and checkout . Astro's **zero-JavaScript-by-default** architecture provides fast page loads and strong SEO via Static Site Generation. **The strongest option for content-heavy storefronts** where SEO and performance outweigh interactivity—not a framework, but a production-ready commerce template.

### General-Purpose Frameworks Used for Commerce

- **[Next.js](https://github.com/vercel/next.js)**  
  React framework with App Router, Server Components, and Server Actions; widely used for headless commerce via Next.js Commerce and custom builds . **The dominant React framework for commerce**, but not commerce-specific—commerce logic comes from Hydrogen or custom API integrations.

- **[Nuxt.js](https://github.com/nuxt/nuxt)**  
  Vue framework with SSR and static generation; commerce modules like `mbl-shop` provide cart, product, and checkout primitives . **The Vue equivalent of Next.js for commerce**, with a smaller but growing headless commerce ecosystem.

- **[Gatsby](https://github.com/gatsbyjs/gatsby)**  
  React static-site framework historically popular for headless commerce via starters and Snipcart integration . **Usage has declined** as Next.js and Astro have gained share; existing Gatsby storefronts remain functional but new projects typically choose alternatives.

- **[Remix](https://github.com/remix-run/remix)**  
  React framework (now merged into React Router) with nested routing and data loading; Shopify's Remix Store is open-source and built with Remix + Hydrogen . **Now part of React Router**, which is one of Hydrogen's supported frameworks.

- **[SvelteKit](https://github.com/sveltejs/kit)**  
  Svelte framework with SSR and static generation; supports headless commerce through adapters and community starters.

- **[Astro](https://github.com/withastro/astro)**  
  Content-focused framework with islands architecture and zero JS by default; commerce templates like Astro Audiophile demonstrate storefront viability .

- **[Angular Universal](https://github.com/angular/universal)**  
  Angular's SSR solution; used for enterprise headless commerce where Angular is the organizational standard. **Niche**—the Angular commerce ecosystem is smaller than React or Vue.

- **[SolidStart](https://github.com/solidjs/solid-start)**  
  SolidJS meta-framework; headless commerce usage remains **experimental** with limited community templates.

### Additional Strong Open-Source Options

- **Saleor Storefront** — React/Next.js storefront for Saleor's GraphQL commerce API; production-grade but tied to Saleor backend .
- **Bagisto Next.js Commerce** — Headless storefront starter connecting Bagisto (Laravel) to Next.js .
- **Vue Storefront (Alokai)** — Frontend-as-a-Service for composable commerce; connects to multiple backends .

**Frameworks for building custom systems**: The framework choice depends on your backend and team. For **Shopify**, use Hydrogen as a library on React Router or Next.js . For **WordPress**, Frontity is the dedicated option . For **multi-backend flexibility**, Svelte Commerce offers the broadest connector coverage . For **content-heavy SEO-first storefronts**, Astro with a commerce template . For **general React/Vue projects**, Next.js or Nuxt.js with commerce modules. The era of commerce-specific frameworks is fading—Hydrogen's library pivot signals that commerce primitives are becoming framework-agnostic, and your framework choice should be driven by team skills and backend, not commerce features.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Headless commerce frameworks handling customer data and transactions must comply with PCI DSS for payments and privacy regulations; the decoupled architecture means security responsibility is distributed across frontend, API, and hosting layers.
- **Open-source headless commerce is mature but in transition**—Hydrogen's shift from framework to library  reflects a broader consolidation: commerce primitives are becoming framework-agnostic, and general-purpose frameworks (Next.js, Nuxt, Astro) are absorbing commerce use cases. Frontity remains the dedicated option for WordPress ; Svelte Commerce offers the broadest multi-backend connectors but with uneven maturity . No single framework is "best"—the right choice depends on your commerce backend and team's framework expertise.
- Verify license terms for commercial use; Hydrogen is open-source (MIT) , Next.js is MIT, Frontity is Apache 2.0, and Svelte Commerce is open-source.

---

**Made for frontend developers, commerce architects, and headless storefront builders.**  
Let's make headless commerce more open, but with clear eyes about the framework consolidation that's reshaping the landscape.
