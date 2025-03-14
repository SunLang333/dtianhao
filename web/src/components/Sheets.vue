<template>
    <v-sheet
      class="d-flex align-center justify-center flex-wrap text-center mx-auto px-4"
      elevation="4"
      max-width="800"
      width="100%"
      rounded
    >
    <MarkdownViewer
        :markdownUrl="markdownUrl"
    />
    </v-sheet>
  </template>
  <script>
  export default {
    name: 'Sheets',
    props: {
      markdownUrl: {
        type: String,
      }
    }
  }
  </script>