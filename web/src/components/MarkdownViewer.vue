<template>
  <div v-html="renderedMarkdown"></div>
</template>

<script>
import { marked } from 'marked';

export default {
  name: 'MarkdownViewer',
  props: {
    markdownContent: {
      type: String,
      default: '',
    },
    markdownUrl: {
      type: String,
      default: '',
    },
  },
  data() {
    return {
      renderedMarkdown: '',
    };
  },
  watch: {
    markdownContent: {
      immediate: true,
      handler(newVal) {
        if (newVal) {
          this.renderedMarkdown = marked(newVal);
        }
      },
    },
    markdownUrl: {
      immediate: true,
      async handler(newVal) {
        if (newVal) {
          try {
            const response = await fetch(newVal);
            const markdown = await response.text();
            this.renderedMarkdown = marked(markdown);
          } catch (error) {
            console.error('Error fetching markdown:', error);
            this.renderedMarkdown = 'Error loading markdown content.';
          }
        }
      },
    },
  },
};
</script>