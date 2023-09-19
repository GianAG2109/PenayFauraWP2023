<template>
    <div>
        
        <v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
			<h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Acerca de nosotros</h1>
		</v-sheet>
        
    <div>
      <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>    
    </div>
    <div class="d-flex align-center flex-column">
      <div class="text-subtitle-2">With props</div>
  
      <v-card
        width="400"
        title="This is a title"
        subtitle="This is a subtitle"
        text="This is content"
      ></v-card>
  
      <div class="mt-4 text-subtitle-2">With slots</div>
  
      <v-card width="400">
        <template v-slot:title>
          This is a title
        </template>
  
        <template v-slot:subtitle>
          This is a subtitle
        </template>
  
        <template v-slot:text>
          This is content
        </template>
      </v-card>
  
      <div class="mt-4 text-subtitle-2">With markup</div>
  
      <v-card width="400">
        <v-card-item>
          <v-card-title>This is a title</v-card-title>
  
          <v-card-subtitle>This is a subtitle</v-card-subtitle>
        </v-card-item>
  
        <v-card-text>
          This is content
        </v-card-text>
      </v-card>
    </div>
    <div>
      <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    </div>
  </template>
<script>
export default{}
</script>