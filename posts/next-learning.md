---
title: "Learning Next"
date: "2020-05-15"
---

What If I Need to Fetch Data at Request Time?
Static Generation is **not** a good idea if you cannot pre-render a page ahead of a user's request. Maybe your page shows frequently updated data, and the page content changes on every request.

In cases like this, you can try **Server-side Rendering** or skipping pre-rendering. Let’s talk about these strategies before we move on to the next lesson.

### Static Generation v.s. Server-side Rendering

We recommend using Static Generation (with and without data) whenever possible because your page can be built once and served by CDN, which makes it much faster than having a server render the page on every request.

## Static Generation

- Static Generation without Data
- Static Generation with Data
  - export async function **getStaticProps**

## Server-side Rendering（blog 不需要这个）

- Server-side Rendering
  - export async function **getServerSideProps**

## Client-side Rendering（possible 的静态 html + 用 js Fetch Data）

It means **Static Generation without Data + Fetch Data on the Client-side using javascript**

## How to Statically Generate Pages with Dynamic Routes

export async function **getStaticPaths**
