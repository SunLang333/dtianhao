<template>
  <v-container class="card-container">
    <Card
      href="https://github.com/SunLang333/kxo302"
      markdownUrl="/kxo302.md"
    />
    <Card
      href="https://github.com/SunLang333/tradingeconomics"
      markdownUrl="/tradingeconomics.md"
    />
    <Card
      href="https://github.com/SunLang333/WebLLM_DeepseekR1"
      markdownUrl="/WebLLM_DeepseekR1.md"
    />
    <Card
      href="https://github.com/SunLang333/DroidCode"
      markdownUrl="/DroidCode.md"
    />
  </v-container>
</template>

<script setup>
import Card from "@/components/Card.vue";

</script>

<style scoped>
.card-container {
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
}
</style>
