<template>
  <v-app>
    <default-bar />
    <Home/>
    <Maps/>
    <FooterView/>
  </v-app>
</template>

<script setup>
  import Home from '@/views/Home.vue';
  import DefaultBar from './AppBar.vue'
  import FooterView from '@/views/FooterView.vue';
  import Maps from '@/views/Maps.vue';
</script>
