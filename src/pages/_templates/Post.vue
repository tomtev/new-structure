---
route: /blog/:title
layout:
  name: SidebarLeft
  props:
    header: false
---

<template>
  <div>
    <h1 v-html="$page.query.post.title"/>
    <div v-html="$page.query.post.content" />
  </div>
</template>

<page-query>
query Post ($path: String!) {
  post: Post (path: $path) {
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