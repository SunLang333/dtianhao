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
        default: 'Vuetify on GitHub'
      },
      subtitle: {
        type: String,
        default: 'Check out the official repository'
      },
      href: {
        type: String,
        default: 'https://github.com'
      },
      markdownUrl: {
        type: String,
        default: 'https://github.com/markdown-it/markdown-it/raw/refs/heads/master/README.md'
      }
    }
  }
  </script>
  