<script setup>
const theme = useCookie("theme");
const component = computed(() => {
    return `LazyThemes${theme.value}Products`
});
</script>

<template>
    <div>
        <component :is="component" />
    </div>
</template>
