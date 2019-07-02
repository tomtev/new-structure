### Normal Pages:
- **Index.vue** is `/` (index.html)
- **Blog.vue** will be `/blog`
- **About.vue** will be `/about`
- **about/History.vue** will be `/about/history`

### Template pages:
Template pages is used for creating single pages for GraphQL types.
Add a **_TypeName[$param].vue** to create pages and routes.

- **_Post[$year][$month][$title].vue** will create pages for **Post** type at `*/:year/:month/:title`.
- **_Author[$name].vue** will create pages for **Author** type  at`*/:name`.
- **_Author[$name][books].vue** will create a sub page for **Author** type at`*/:name/books`.


### Dynamic pages:
- **account/$user.vue** creates dynamic `account/:user` url with access to **$route.param.user**.

This will generate a `acccount/user.html` file that all dynamic routes should do a 200 redirect to. You can do this automatically for Netlify and Zeit with plugins.
