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

</v-card>
    <br>
  </template>
  
  <script>
import MarkdownViewer from './MarkdownViewer.vue';

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
        default: 'https://github.com/vuetifyjs/vuetify/'
      }
    }
  }
  </script>
  