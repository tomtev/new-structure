<template>
  <div>
    <h1 v-html="$page.query.post.title"/>
    <div v-html="$page.query.post.content" />
  </div>
</template>

<page-query>
query Post ($id: String!) {
  post: Post (id: $id) {
    title
    date (format: "D. MMMM YYYY")
    timeToRead
    content
    author {
      id
      title
      path,
      avatar (width: 60)
    }
    excerpt
  }
}
</page-query>