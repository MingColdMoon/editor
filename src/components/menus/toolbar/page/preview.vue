<template>
  <menus-button
    v-if="page.preview.isShow"
    ico="preview"
    :text="t('page.preview')"
    huge
    :menu-active="page.preview.enabled"
    @menu-click="page.preview.enabled = !page.preview.enabled"
  />
</template>

<script setup lang="ts">
const page = inject('page')
</script>
