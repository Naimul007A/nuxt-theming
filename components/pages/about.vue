<script setup>
const theme = useCookie("theme");
const component = computed(() => {
    return `LazyThemes${theme.value}About`
});
</script>
<template>
    <div>
        <component :is="component" />
    </div>
</template>

<style lang="scss" scoped></style>
