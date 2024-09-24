<script setup>
import { LazyThemesShopus, LazyThemesDefault, LazyThemesBoibazar } from "#components";
const theme = useCookie("theme");
const component = computed(() => {
    switch (theme.value.toLowerCase()) {
        case "shopus":
            return LazyThemesShopus;
        case "boibazar":
            return LazyThemesBoibazar;
        default:
            return LazyThemesDefault;
    }
});

</script>
<template>
    <div>
        <component :is="component" />
    </div>
</template>
