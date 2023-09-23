<template>
    <div>
        <v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
		    <h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Socios</h1>
		</v-sheet>      
    </div>
    
    <div>
        <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>



<v-row align="center" justify="center">
    <div>
    <!--Doctor Peña-->
    <v-col>
                <v-card
            class="mx-auto"
            max-width="344"
        >
        <v-img
            src="../assets/Socios/drpena.jpg"
            height="200px"
            cover
        ></v-img>

        <v-card-title>
            Mariano Peña Benavides
        </v-card-title>

        <v-card-subtitle>
            Teléfonos Fijos : (511) 447-3853  (511) 444-7906
        </v-card-subtitle>
        <v-card-subtitle>
            Móvil : (51) 999377748
        </v-card-subtitle>
        <v-card-subtitle>
            Correo : mapena@penayfaura.com
        </v-card-subtitle>

        <v-card-actions>

        <v-spacer></v-spacer>

        <v-btn
            :icon="show1 ? 'mdi-chevron-up' : 'mdi-chevron-down'"
            @click="show1 = !show1"
        ></v-btn>
        </v-card-actions>

        <v-expand-transition>
        <div v-show="show1">
        <v-divider></v-divider>

        <v-card-text>
            Abogado egresado de la Universidad Particular San Martín de Porres de Lima, Perú, con estudios de Maestría en Derecho Internacional Económico en la Pontificia Universidad Católica del Perú. Arbitro registrado en la Cámara de Comercio de Lima y de la Cámara de Arbitraje de la Pontificia Universidad Católica del Perú. Es miembro mayor y Directivo del Capítulo Peruano de la Federación Interamericana de Abogados; representante ante el grupo ABRIL. Especialista en Derecho Corporativo y Derecho Internacional Privado.
            Idiomas: Español, Inglés.
        </v-card-text>
      </div>

      

        </v-expand-transition>
    </v-card>
    </v-col>
</div>
<div>
    <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
</div>
<div>
    <!--Doctor Faura-->
    <v-col>
                <v-card
            class="mx-auto"
            max-width="344"
        >
        <v-img
            src="../assets/Socios/DrFaura.jpg"
            height="200px"
            cover
        ></v-img>

        <v-card-title>
            Manuel Faura Bermúdez
        </v-card-title>

        <v-card-subtitle>
            Teléfonos Fijos : (511) 447-3853  (511) 242-8640
        </v-card-subtitle>
        <v-card-subtitle>
            Móvil : (51) 999277207
        </v-card-subtitle>
        <v-card-subtitle>
            Correo : mfaura@penayfaura.com
        </v-card-subtitle>

        <v-card-actions>

        <v-spacer></v-spacer>

        <v-btn
            :icon="show2 ? 'mdi-chevron-up' : 'mdi-chevron-down'"
            @click="show2 = !show2"
        ></v-btn>
        </v-card-actions>

        <v-expand-transition>
        <div v-show="show2">
        <v-divider></v-divider>

        <v-card-text>
            Abogado egresado de la Pontificia Universidad Católica del Perú con estudios de Maestría en Derecho Empresarial en la Universidad de Lima. Ha sido profesor en la Pontificia Universidad Católica del Perú, Universidad de Lima y Universidad Femenina del Sagrado Corazón; miembro mayor de la Federación Interamericana de Abogados – FIA. Fue Procurador Público del Ministerio de Trabajo (1995) y Vocal de la Primera Sala Laboral Permanente de Lima (1996). Árbitro con Registro del Ministerio de Trabajo y Promoción del Empleo. Sectores público y privado. Especialista en Derecho Laboral.
            Idiomas: Español, Inglés.


        </v-card-text>
      </div>

      

        </v-expand-transition>
    </v-card>
    </v-col>
</div>       
<div>
    <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
</div>

<div>
 <!--Doctor Arnaiz-->
 <v-col>
             <v-card
             class="mx-auto"
         max-width="344"
         
     >
     <v-img
         src="../assets/Socios/arnaiz2.jpg"
         height="200px"
         cover
     ></v-img>

     <v-card-title>
        Susana Arnaiz Jibaja
     </v-card-title>

     <v-card-subtitle>
        Teléfonos Fijos : (511) 447-3853  (511) 444-7906
     </v-card-subtitle>

     <v-card-subtitle>
        Móvil : (51) 980101261
     </v-card-subtitle>
     <v-card-subtitle>
         Correo : suarnaiz@penayfaura.com
     </v-card-subtitle>

     <v-card-actions>

     <v-spacer></v-spacer>

     <v-btn
         :icon="show3 ? 'mdi-chevron-up' : 'mdi-chevron-down'"
         @click="show3 = !show3"
     ></v-btn>
     </v-card-actions>

     <v-expand-transition>
     <div v-show="show3">
     <v-divider></v-divider>

     <v-card-text>
        Estudió Derecho en la Pontificia Universidad Católica del Perú y realizó estudios adicionales de Derecho en la Universidad Rafael Landívar de Guatemala. Es docente en temas de Derecho y Comercio Internacional, en el Instituto Superior Tecnológico Peruano Alemán Alexander Von Humboldt. Especialista en Derecho Corporativo, Derecho de la Propiedad Intelectual y Derecho de la Competencia.
Idiomas: Español, Inglés, Alemán
     </v-card-text>
   </div>

   

     </v-expand-transition>
 </v-card>
 </v-col>
</div>

<div>
    <v-divider :thickness="20" class="border-opacity-0" vertical></v-divider>
</div>


 <div>
 <!--Doctor Moscoso-->
 <v-col>
             <v-card
         class="mx-auto"
         max-width="344"
     >
     <v-img
         src="../assets/Socios/Dr-Moscoso.jpg"
         height="200px"
         cover
     ></v-img>

     <v-card-title>
        Luis Moscoso Delgado
     </v-card-title>

     <v-card-subtitle>
         Teléfonos Fijos : (511) 447-3853
                         (511) 242-8052
     </v-card-subtitle>
     <v-card-subtitle>
         Móvil : (51) 980101261
     </v-card-subtitle>
     <v-card-subtitle>
         Correo : lmoscoso@penayfaura.com
     </v-card-subtitle>

     <v-card-actions>

     <v-spacer></v-spacer>

     <v-btn
         :icon="show4 ? 'mdi-chevron-up' : 'mdi-chevron-down'"
         @click="show4 = !show4"
     ></v-btn>
     </v-card-actions>

     <v-expand-transition>
     <div v-show="show4">
     <v-divider></v-divider>

     <v-card-text>
         Abogado egresado de la Universidad Particular San Martín de Porres de Lima, Perú, con estudios de Maestría en Derecho Internacional Económico en la Pontificia Universidad Católica del Perú. Arbitro registrado en la Cámara de Comercio de Lima y de la Cámara de Arbitraje de la Pontificia Universidad Católica del Perú. Es miembro mayor y Directivo del Capítulo Peruano de la Federación Interamericana de Abogados; representante ante el grupo ABRIL. Especialista en Derecho Corporativo y Derecho Internacional Privado.
         Idiomas: Español, Inglés.
     </v-card-text>
   </div>

   

     </v-expand-transition>
 </v-card>
 </v-col>
</div>
</v-row>








 




    
    <div>
        <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>









    



</template>
<script>
  export default {
    data: () => ({
      show1: false,
      show2: false,
      show3: false,
      show4: false,
    }),
  }
</script>