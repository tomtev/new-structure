### Normal Pages:
- **/Index.vue** is `/` (index.html)
- **/blog/Index.vue** will be `/blog`
- **/About.vue** will be `/about`
- **/about/Vision.vue** will be `/about/vision`

### Source pages:
Source pages is used for creating single pages for data collections.
Add a **_TypeName[$param].vue** to create pages and routes.

- **/blog/_Post[$title].vue** will create pages for **Post** type at `blog/:title`.
- **/blog/_Post[$year][$month][$title].vue** will create pages for **Post** type at `blog/:year/:month/:title`.
- **/authors/_Author[$name].vue** will create pages for **Author** type  at`authors/:name`.
- **/authors/_Author[$name][books].vue** will create a sub page for **Author** type at`authors/:name/books`.

### Dynamic pages:
- **/account/$user.vue** creates a dynamic `/account/:user` url with access to **$route.param.user**.

This will generate a `acccount/user.html` file that all dynamic routes should do a 200 redirect to. You can do this automatically for Netlify and Zeit with plugins.
