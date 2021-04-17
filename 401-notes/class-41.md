# React 3

**LINKS**

- [Next.js - Dynamic Routes](https://nextjs.org/learn/basics/dynamic-routes)
- [Next.js - Deployment](https://nextjs.org/learn/basics/deploying-nextjs-app)
- [Next.js 10 is here](https://www.youtube.com/watch?v=JWCS5IdECVI)
- [Next.js - Static File Serving](https://nextjs.org/docs/basic-features/static-file-serving)

## Next.js - Dynamic Routes

We can do this by taking the following steps. You don’t have to make these changes yet — we’ll do it all on the next page.

First, we’ll create a page called `[id].js` under `pages/posts`. Pages that begin with `[` and end with `]` are dynamic routes in Next.js.

In `pages/posts/[id].js`, we’ll write code that will render a post page — just like other pages we’ve created.

```JavaScript
import Layout from '../../components/layout'

export default function Post() {
  return <Layout>...</Layout>
}
```

## Deploying Your Next.js App to Vercel

The easiest way to deploy Next.js to production is to use the Vercel platform developed by the creators of Next.js.

Vercel is an all-in-one platform with Global CDN supporting static & JAMstack deployment and Serverless Functions. We believe Vercel is the optimal place to deploy Next.js apps. You can start using it for free — no credit card required.

**Create a Vercel Account**

Vercel is made by the creators of Next.js and has first-class support for Next.js. When you deploy your Next.js app to Vercel, the following happens by default:

Pages that use Static Generation and assets (JS, CSS, images, fonts, etc) will automatically be served from the Vercel Edge Network, which is blazingly fast.
Pages that use Server-Side Rendering and API routes will automatically become isolated Serverless Functions. This allows page rendering and API requests to scale infinitely.
Vercel has many more features, such as:

Custom Domains: Once deployed on Vercel, you can assign a custom domain to your Next.js app. Take a look at our documentation here.
Environment Variables: You can also set environment variables on Vercel. Take a look at our documentation here. You can then use those environment variables in your Next.js app.
Automatic HTTPS: HTTPS is enabled by default (including custom domains) and doesn't require extra configuration. We auto-renew SSL certificates.
You can learn more about the platform in the Vercel documentation.

[Back to Homepage](https://ashcaz.github.io/reading-notes)
