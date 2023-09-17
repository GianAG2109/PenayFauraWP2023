<template>
    <div>
        <v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
			<h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Servicios</h1>
		</v-sheet>
    </div>
    <div>
        <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>
    <div>
        
        <v-row>
            <v-col>
                <ServiciosPYF/>
            </v-col>
            <v-divider class="border-opacity-0" vertical></v-divider>
            <v-col>
                <ServiciosPYF2/>
            </v-col>
        </v-row>
    </div>
    <div>
        <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>


</template>
<script setup>
import ServiciosPYF from '@/components/ServiciosPYF.vue';
import ServiciosPYF2 from '@/components/ServiciosPYF2.vue'
</script>