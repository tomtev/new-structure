---
title: Our Blog
layout: SidebarLeft
---

<template>
  <div>
   	<h1>{{ $page.title }}</h1>
   	
   	<div v-for="post in $page.query.posts">
   		...posts
   	</div>

   	<template slot="sidebar">
   		Går dette?
   	</template>
  </div>
</template>

<page-query>
query Posts {
  posts: allPost {
    edges {
      node {
        id
        title
        path
        date (format: "D. MMMM YYYY")
        timeToRead
        author {
          title
          path
          avatar (width: 60)
        }
        excerpt
        content
      }
    }
  }
}
</page-query>