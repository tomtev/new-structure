---
title: $page.query.post.title
route: /tags/:title
layout: SidebarLeft
---

<template>
  <div>
    <h1 v-html="$page.title"/>
    <div v-html="$page.query.post.content" />
  </div>
</template>

<page-query>
query Post ($id: String!) {
  post: Post (id: $path) {
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