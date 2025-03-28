## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

- Clone the repo
- Run `pnpm install` to install the dependencies
- Run `pnpm dev` to start the development server
- Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### Summary

To recap, we have done a few things to optimize data fetching in our application so far:

1. Created a database in the same region as your application code to reduce latency between your server and database.
2. Fetched data on the server with React Server Components. This allows you to keep expensive data fetches and logic on the server, reduces the client-side JavaScript bundle, and prevents your database secrets from being exposed to the client.
3. Used SQL to only fetch the data you needed, reducing the amount of data transferred for each request and the amount of JavaScript needed to transform the data in-memory.
4. Parallelize data fetching with JavaScript - where it made sense to do so.
5. Implemented Streaming to prevent slow data requests from blocking your whole page, and to allow the user to start interacting with the UI without waiting for everything to load ( by using loading.tsx file ).
6. Move data fetching down to the components that need it, thus isolating which parts of your routes should be dynamic.
