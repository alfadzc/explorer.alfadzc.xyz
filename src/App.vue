<script setup lang="ts">
import { themeChange } from 'theme-change';
import { onMounted } from 'vue';
import TxDialog from './components/TxDialog.vue';
import LoadingScreen from './components/LoadingScreen.vue';

onMounted(() => {
  themeChange(false);
});
</script>

<template>
  <div>
    <LoadingScreen />
    <RouterView />
    <TxDialog />
  </div>
</template>
