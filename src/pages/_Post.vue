---
route: /blog/:title
title: $page.query.post.title
layout: SidebarLeft
appProps: {transparent: $page.query.post.transparent}
---

<template>
  <div>
    <h1 v-html="$page.title"/>
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