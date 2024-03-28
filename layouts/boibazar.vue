<script setup>
// setup script
</script>

<template>
  <div>hello {{ useCookie("theme") }}</div>
  <themes-boibazar-header />
  <slot />
  <themes-boibazar-footer />
</template>

<style scoped>
/* scoped style  */
</style>
