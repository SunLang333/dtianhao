<template>
    <v-card
      append-icon="mdi-open-in-new"
      class="mx-auto"
      :href="href"
      max-width="344"
      prepend-icon="mdi-github"
      rel="noopener"
      :subtitle="subtitle"
      target="_blank"
      :title="title"
    >
    <MarkdownViewer
        :markdownUrl="markdownUrl"
    />
    </v-card>
    <br>
  </template>
  
  <script>

  export default {
    name: 'CustomCard',
    props: {
      title: {
        type: String,
      },
      subtitle: {
        type: String,
      },
      href: {
        type: String,
      },
      markdownUrl: {
        type: String,
      }
    }
  }
  </script>
  <style>
img {
    width:-webkit-fill-available
}
  </style>
  