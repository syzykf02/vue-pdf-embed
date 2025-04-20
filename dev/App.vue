<script setup lang="ts">
import VuePdfEmbed from '../src/index'

const pdfSource = '大语言模型的幻觉问题研究综述.pdf'
</script>

<template>
  <VuePdfEmbed annotation-layer text-layer :source="pdfSource" />
</template>

<style lang="scss">
@import 'pdfjs-dist/web/pdf_viewer.css';

body {
  padding: 16px;
  background-color: #a8a7a7;
}

.vue-pdf-embed {
  margin: auto;
  max-width: 1024px;

  & > div {
    margin-bottom: 4px;
    box-shadow: 0 2px 8px 4px rgba(0, 0, 0, 0.1);
  }
}
</style>
