### Normal Pages:
- **Index.vue** is /
- **Blog.vue** will be /blog
- **About.vue** will be /about
- **about/History.vue** will be /about/history


### Template pages:
Template pages is used for creating single-page templates for GraphQL types.
- **_template/Post.vue** gets data from `Post` GraphQL type.
- **_template/Portfolio.vue** gets data from `Portfolio` GraphQL type.
### Dynamic pages:
- **account/$user.vue** creates dynamic `account/:user` url with access to $route.user param.

You can delete this file.
