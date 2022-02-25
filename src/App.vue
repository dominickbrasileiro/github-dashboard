<script setup lang="ts">
import { ref } from "vue";

const isDrawerOpen = ref(true);
</script>

<template>
  <q-layout view="hHh lpR fFf">
    <q-header elevated class="bg-dark text-white">
      <q-toolbar>
        <q-toolbar-title> GitHub Dashboard </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer v-model="isDrawerOpen" bordered> </q-drawer>
  </q-layout>
</template>
