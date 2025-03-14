<template>
  <v-layout class="overflow-visible" style="height: 56px;">
    <v-bottom-navigation
      v-model="value"
      color="teal"
      grow
    >
      <v-btn>
        <v-icon>mdi-history</v-icon>

        Recents
      </v-btn>

      <v-btn>
        <v-icon>mdi-file-document</v-icon>

        Resume
      </v-btn>

      <v-btn>
        <v-icon>mdi-account-plus</v-icon>

        Contact Me
      </v-btn>
    </v-bottom-navigation>
  </v-layout>
</template>
<script setup>
  import { ref } from 'vue'

  const value = ref(1)
</script>