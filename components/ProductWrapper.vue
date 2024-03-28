<script setup>
import ThemesBoibazarProductWrapper from "@/components/themes/boibazar/ProductWrapper";
import ThemesShopusProductWrapper from "@/components/themes/shopus/ProductWrapper";
import ThemesDefaultProductWrapper from "@/components/themes/default/ProductWrapper";
const theme = useCookie("theme");
let ProductWrapper;
switch (theme) {
  case "boibazar":
    ProductWrapper = ThemesBoibazarProductWrapper;
    break;
  case "shopus":
    ProductWrapper = ThemesShopusProductWrapper;
    break;
  default:
    ProductWrapper = ThemesDefaultProductWrapper;
}
</script>

<template>
  <div>
    <h1>{{ theme }} Product Wrapper</h1>
    <component :is="ProductWrapper" />
  </div>
</template>
