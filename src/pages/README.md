### Normal Pages:
- **Index.vue** is /
- **Blog.vue** will be /blog
- **About.vue** will be /about
- **about/History.vue** will be /about/history


### Template pages:
Template pages is used for creating single-page templates for GraphQL types. These can be added anywhere.

- **_Post[$year][$month][$title]** will create pages for **Post** type `folder/:year/:month/:title`.
- **_Author[$name]** will create pages for **Author** type  at`folder/:name`.
- **_Author[$name][books]** will sub pages for **Author** type at`folder/:name/books`.


### Dynamic pages:
- **account/$user.vue** creates dynamic `account/:user` url with access to **$route.param.user**.

You can delete this file.
