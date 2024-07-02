## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.


### Routing

Next.js uses file-structure routing

```
---app
    ---layout.tsx
    ---page.tsx
    ---dashboard
        ---page.tsx
        ---layout.tsx
        ---customer
            ---page.tsx
            ---layout.tsx
        ---invoices
            ---page.tsx
```

`page.tsx` : is the index page of coresponding route.

`layout.tsx` : create UI that is shared between multiple pages. The `<Layout />` component receives a children prop. 
This child can either be a page or another layout. In your case, the pages inside /dashboard will automatically be nested inside a `<Layout />`.

### Navigating Between Pages

`<Link/>` : In Next.js, you can use the `<Link />` Component to link between pages in your application.`<Link>` allows you to do client-side navigation with JavaScript.

**Next.js automatically prefetches** the code for the linked route in the background. By the time the user clicks the link, the code for the destination page will already be loaded in the background, and this is what makes the page transition near-instant!

`'use client'`
- Client Components: These are components that are rendered on the client side (browser). They can utilize hooks like useState and useEffect, interact with the DOM, and handle     client-specific logic.
- Server Components: These are components that are rendered on the server. They are typically used to fetch data and render HTML, which is then sent to the client. They do not have access to browser-specific APIs or React hooks like `useState` and `useEffect`.










