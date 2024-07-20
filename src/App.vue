<script setup>
import HomepageView from './views/HomepageView.vue'

const isDesktop = window.innerWidth > 1024
const isTablet = window.innerWidth <= 1024 && innerWidth > 7487
</script>

<template>
  <template v-if="isDesktop">
    <HomepageView />
  </template>
  <template v-else-if="isTablet">This is tablet</template>
  <template v-else>
    <div v-show="!isDesktop && !isTablet">this is mobile</div>
  </template>
  <div v-show="!isDesktop && !isTablet">this is mobile</div>
</template>
