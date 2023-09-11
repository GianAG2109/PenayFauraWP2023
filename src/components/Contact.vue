<template>
    <v-divider class="border-opacity-0" vertical></v-divider>
    <v-divider class="border-opacity-0" vertical></v-divider>
    <div>
        
        <v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
			<h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Contactenos</h1>
		</v-sheet>
        
        
    </div>
    <v-divider class="border-opacity-0" vertical></v-divider>
   
    
    <div>
        <v-row>
            <v-col>
                <v-sheet
                    class="d-flex align-center justify-center flex-wrap text-center mx-auto px-4"
                    elevation="4"
                    height="250"
                    rounded
                    max-width="800"
                    width="90%"
                >
                <div>
                    <h2 class="text-h5 font-weight-black text-red">Contactenos</h2>
                    <v-car>
                              <v-form v-model="valid">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          md="4"
        >
          <v-text-field
            v-model="firstname"
            :rules="nameRules"
            :counter="10"
            label="First name"
            required
            hide-details
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          md="4"
        >
          <v-text-field
            v-model="lastname"
            :rules="nameRules"
            :counter="10"
            label="Last name"
            hide-details
            required
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          md="4"
        >
          <v-text-field
            v-model="email"
            :rules="emailRules"
            label="E-mail"
            hide-details
            required
          ></v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
                    </v-car>
                </div>
                </v-sheet>
            </v-col>
            <v-divider class="border-opacity-0" vertical></v-divider>
            <v-col>
                <v-sheet
                    class="d-flex align-center justify-center flex-wrap text-center mx-auto px-4"
                    elevation="4"
                    height="250"
                    rounded
                    max-width="800"
                    width="90%"
                >
                <div>
                    





                    <h2 class="text-h5 font-weight-black text-red">Peña &amp;&nbsp;Faura – Asesores Consultores</h2>

                    <strong>Dirección:</strong>&nbsp;Av. Alfredo Benavides 2150, Of. 402, Miraflores, Lima &#8211; Perú
                    <strong>Socios:</strong>
                    <h4>Mariano Peña Benavides</h4>
                    <h4>Manuel Faura Bermúdez</h4>
                    <h4>Susana Arnaiz Jibaja</h4>
                    <h4>Luis Moscoso Delgado</h4>


                </div>
                </v-sheet>
            </v-col>
        </v-row>
    </div>
    <v-divider class="border-opacity-0"></v-divider>
    <v-divider class="border-opacity-0"></v-divider>
    <v-divider class="border-opacity-0"></v-divider>
    <v-divider class="border-opacity-0"></v-divider>

</template>
<script>
  export default {
    data: () => ({
      valid: false,
      firstname: '',
      lastname: '',
      nameRules: [
        value => {
          if (value) return true

          return 'Name is required.'
        },
        value => {
          if (value?.length <= 10) return true

          return 'Name must be less than 10 characters.'
        },
      ],
      email: '',
      emailRules: [
        value => {
          if (value) return true

          return 'E-mail is requred.'
        },
        value => {
          if (/.+@.+\..+/.test(value)) return true

          return 'E-mail must be valid.'
        },
      ],
    }),
  }
</script>