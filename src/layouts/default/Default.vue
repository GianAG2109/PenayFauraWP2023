<template>
  <v-app> 
    <default-bar />
    <Home/>
    <AcercaDeNosotros/>
    <SociosVue/>
    <Servicios/>
    <Contactenos/>


    <Maps/>
    <FooterView/>
    
  </v-app>
</template>

<script setup>

  import Home from '@/views/Home.vue';
  import DefaultBar from './AppBar.vue'
  import FooterView from '@/views/FooterView.vue';
  import Maps from '@/views/Maps.vue';
  import Contactenos from '@/views/Contactenos.vue';
import AcercaDeNosotros from '@/views/AcercaDeNosotros.vue';
import SociosVue from '@/views/Socios.vue';
import Servicios from '@/views/Servicios.vue';

</script>
