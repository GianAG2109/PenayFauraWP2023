<template>

    <v-responsive class="border pa-4">
      
    <div>
      <v-row>
 
        <v-col>
          
            <v-responsive class="border pa-4">
            <v-textarea label="Label"></v-textarea>
          </v-responsive>
          
        </v-col>
        <v-divider class="border-opacity-0" vertical></v-divider>
        <v-col>
          <v-card text="..."></v-card>
        </v-col>
      </v-row>
    </div>
  

  </v-responsive>

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