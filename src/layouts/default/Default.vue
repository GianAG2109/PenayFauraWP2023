<template>
  <v-app> 
    <default-bar />
    <Home/>
    <AcercaDeNosotros/>
    <SociosVue/>
    <Servicios/>
    <v-responsive class="border pa-4">
    <div>
      <v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
			  <h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Contactenos</h1>
        
		  </v-sheet>
    </div>
    <Contactenos/>
    </v-responsive>
    


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
