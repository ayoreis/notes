## Rendering

Data + Code = HTML

Server-side caching
Client-side caching

## Factors, considerations

### User experience (UX)

The user may be a human, a crawler or a preview, SEO

- Core Web Vitals

### Developer experience (DX)

- Fast builds
- Low costs
- ...

## Where

- Server [Web server - Wikipedia](https://en.wikipedia.org/wiki/Web_server)
- CDN [Content delivery network - Wikipedia](https://en.wikipedia.org/wiki/Content_delivery_network)
- Edge [Edge computing - Wikipedia](https://en.wikipedia.org/wiki/Edge_computing)

Which may be serverless [Serverless computing - Wikipedia](https://en.wikipedia.org/wiki/Serverless_computing)

## Static rendering

[Static web page - Wikipedia](https://en.wikipedia.org/wiki/Static_web_page)

HTML generated at build time
easily cacheablen in a CDN or Edge Network
do not contain request-based data

### Hand writing

Good old HTML

### Static site generator (SSG)

[Static site generator - Wikipedia](https://en.wikipedia.org/wiki/Static_site_generator)

For example Markdown -> HTML

### Jamstack

[WTF is Jamstack?](https://jamstack.wtf)
[Jamstack - Wikipedia](https://en.wikipedia.org/wiki/Jamstack)

### ISR

[Incremental Static Regeneration (ISR) | Vercel Docs](https://vercel.com/docs/incremental-static-regeneration)
[Data Fetching: Incremental Static Regeneration | Next.js](https://nextjs.org/docs/pages/building-your-application/data-fetching/incremental-static-regeneration)

Can be trigered by a timer or a hook

## Server-side rendering (SSR)

[Server-side scripting - Wikipedia](https://en.wikipedia.org/wiki/Server-side_scripting)
[Dynamic web page - Wikipedia](https://en.wikipedia.org/wiki/Dynamic_web_page)

Fully render page _when requested_, that is important, the client may only request it once

### Streaming

server -> client

## Client-side rendering (CSR)

## Hydration

partial
progressive
selective

### Islands

## Resumability

---

    ## Multi-page app (MPA)

    Every navigation is a full page load

    May be hydarted or resumed by client

## Single-page app (SPA)

Navigation is handled by client

but isent plain stuff better, this is fater (eg preload on hover)

~~Shell or skeleton HTML is hydrated by JavaScript~~

May have client side navigation/routing

[Single-page application - Wikipedia](https://en.wikipedia.org/wiki/Single-page_application)
