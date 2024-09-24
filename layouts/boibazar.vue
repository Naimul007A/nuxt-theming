<script setup>
// setup script
</script>

<template>
  <div>hello {{ useCookie("theme") }}</div>
  <themes-boibazar-utils-header />
  <slot />
  <themes-boibazar-utils-footer />
</template>

<style scoped>
/* scoped style  */
</style>
