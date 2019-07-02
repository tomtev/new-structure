### Normal Pages:
- **Index.vue** is /
- **Blog.vue** will be /blog
- **About.vue** will be /about
- **about/History.vue** will be /about/history


### Template pages:
Template pages is used for creating single-page templates for GraphQL types. These can be added anywhere.

- **_Collection[$title]** will create pages from collection at `folder/:title`.
- **_Collection[$title][books]** will create pages from collection at `folder/:title/books`.


### Dynamic pages:
- **account/$user.vue** creates dynamic `account/:user` url with access to $route.user param.

You can delete this file.
