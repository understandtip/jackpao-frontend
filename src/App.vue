<script setup lang="ts">
import BasicLayout from "./layouts/BasicLayout.vue";
import { useRoute } from "vue-router";

const route = useRoute();
</script>

<template>
  <div>
    <template v-if="route.path.startsWith('/user/login')">
      <router-view />
    </template>
    <template v-else>
      <BasicLayout />
    </template>
  </div>
</template>

<style>

</style>
