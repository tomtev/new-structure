### Normal Pages:
- **Index.vue** is `/` (index.html)
- **Blog.vue** will be `/blog`
- **About.vue** will be `/about`
- **about/History.vue** will be `/about/history`

### Source pages:
Source pages is used for creating single-page templates for GraphQL types.

- **_Post[$year][$month][$title].vue** will create pages for **Post** type at `*/:year/:month/:title`.
- **_Author[$name].vue** will create pages for **Author** type  at`*/:name`.
- **_Author[$name][books].vue** will create a sub page for **Author** type at`*/:name/books`.


### Dynamic pages:
- **account/$user.vue** creates dynamic `account/:user` url with access to **$route.param.user**.

You can delete this file.
