<script setup lang="ts">
import { ref } from "vue";

const isDrawerOpen = ref(true);

const toggleDrawer = () => {
  isDrawerOpen.value = !isDrawerOpen.value;
};
</script>

<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-dark text-white">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="toggleDrawer" />

        <q-toolbar-title> GitHub Dashboard </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer show-if-above bordered side="left" v-model="isDrawerOpen" />
  </q-layout>
</template>
