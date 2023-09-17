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

        <v-row>
          <v-col>
            <v-card title="Contactenos" text=" "           class="mx-auto"
            max-width="600">
            <v-sheet width="400" class="mx-auto">

<v-form ref="form">
  <v-text-field
    v-model="name"
    :counter="10"
    :rules="nameRules"
    label="Name"
    required
  ></v-text-field>

  <v-select
    v-model="select"
    :items="items"
    :rules="[v => !!v || 'Item is required']"
    label="Item"
    required
  ></v-select>

  <v-checkbox
    v-model="checkbox"
    :rules="[v => !!v || 'You must agree to continue!']"
    label="Do you agree?"
    required
  ></v-checkbox>

  <div class="d-flex flex-column">
    <v-btn
      color="success"
      class="mt-4"
      block
      @click="validate"
    >
      Validate
    </v-btn>

    <v-btn
      color="error"
      class="mt-4"
      block
      @click="reset"
    >
      Reset Form
    </v-btn>
  </div>
</v-form>
</v-sheet>
            </v-card>
          </v-col>
          <v-divider class="border-opacity-0" vertical></v-divider>
          <v-col>
            <v-card title="Card title" text="..." class="mx-auto" max-width="600">

            </v-card>
          </v-col>
        </v-row>
      
    </div>
    <div>
      <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>
</template>
<script>
  export default {
    data: () => ({
      name: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => (v && v.length <= 10) || 'Name must be less than 10 characters',
      ],
      select: null,
      items: [
        'Item 1',
        'Item 2',
        'Item 3',
        'Item 4',
      ],
      checkbox: false,
    }),

    methods: {
      async validate () {
        const { valid } = await this.$refs.form.validate()

        if (valid) alert('Form is valid')
      },
      reset () {
        this.$refs.form.reset()
      },
      resetValidation () {
        this.$refs.form.resetValidation()
      },
    },
  }
</script>