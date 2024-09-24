<script setup lang="ts">
const theme = useCookie("theme");
theme.value = "Shopus";
const mytheme = theme.value.toLowerCase();
</script>
<template>
  <NuxtLayout :name="mytheme">
    <NuxtPage />
  </NuxtLayout>
</template>
