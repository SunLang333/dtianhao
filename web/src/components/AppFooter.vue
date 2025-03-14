<template>
  <v-layout class="overflow-visible" style="height: 56px;">
    <v-bottom-navigation
      color="teal"
      grow
    >
      <router-link to="/">
        <v-btn>
          <v-icon>mdi-home</v-icon>

          Recents
        </v-btn>
      </router-link>

      <router-link to="/resume">
        <v-btn>
          <v-icon>mdi-file-document-edit</v-icon>

          Resume
        </v-btn>
      </router-link>
      <router-link to="/contact">
      <v-btn>
        <v-icon>mdi-account-plus</v-icon>

        Hire!Me!
      </v-btn>
    </router-link>
    </v-bottom-navigation>
  </v-layout>
</template>
<script setup></script>