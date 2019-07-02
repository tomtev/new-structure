### Normal Pages:
- **Index.vue** is `/` (index.html)
- **Blog.vue** will be `/blog`
- **About.vue** will be `/about`
- **about/History.vue** will be `/about/history`


### Data pages:
Data pages is used for creating single pages for GraphQL types.

- **_Post[$year][$month][$title]** will create pages for **Post** type at `folder/:year/:month/:title`.
- **_Author[$name]** will create pages for **Author** type  at`folder/:name`.
- **_Author[$name][books]** will sub pages for **Author** type at`folder/:name/books`.


### Dynamic pages:
- **account/$user.vue** creates dynamic `account/:user` url with access to **$route.param.user**.

You can delete this file.
