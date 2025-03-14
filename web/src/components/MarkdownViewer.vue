<template>
  <div v-if="!error" v-html="renderedMarkdown"></div>
  <div v-else class="error-message">Error: {{ error }}</div>
</template>

<script>
import MarkdownIt from 'markdown-it';

export default {
  name: 'MarkdownViewer',
  props: {
    markdown: {
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
      error: null,
      markdownContent: '',
      md: null,
    };
  },
  async mounted() {
    this.md = new MarkdownIt();
    if (this.markdownUrl) {
      try {
        const response = await fetch(this.markdownUrl);
        if (!response.ok) {
          throw new Error(`HTTP error! status: ${response.status}`);
        }
        this.markdownContent = await response.text();
      } catch (error) {
        this.error = error.message;
      }
    } else {
      this.markdownContent = this.markdown;
    }
  },
  computed: {
    renderedMarkdown() {
      if (this.md && this.markdownContent) {
        return this.md.render(this.markdownContent);
      }
      return '';
    }
  },
};
</script>