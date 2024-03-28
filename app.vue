<script setup lang="ts">
const theme = useCookie("theme");
theme.value = "default";
const mytheme = theme.value;
</script>
<template>
  <NuxtLayout :name="mytheme">
    <NuxtPage />
  </NuxtLayout>
</template>
