<template>
  
    <div>
      <v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
			  <h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Contactenos</h1>
		  </v-sheet>
    </div>
    <div>
        <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>
    <div>
          <v-divider class="border-opacity-0" vertical></v-divider>
    </div>
    <div>
      <v-row>
 
        <v-col>
          <v-card text="..."></v-card>
        </v-col>
        <v-divider class="border-opacity-0" vertical></v-divider>
        <v-col>
          <v-card text="..."></v-card>
        </v-col>
      </v-row>
    </div>
    <div>
        <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>
</template>
<script>
  export default {
    data: vm => ({
      loading: false,
      rules: [value => vm.checkApi(value)],
      timeout: null,
      userName: '',
    }),

    methods: {
      async submit (event) {
        this.loading = true

        const results = await event

        this.loading = false

        alert(JSON.stringify(results, null, 2))
      },
      async checkApi (userName) {
        return new Promise(resolve => {
          clearTimeout(this.timeout)

          this.timeout = setTimeout(() => {
            if (!userName) return resolve('Please enter a user name.')
            if (userName === 'johnleider') return resolve('User name already taken. Please try another one.')

            return resolve(true)
          }, 1000)
        })
      },
    },
  }
</script>