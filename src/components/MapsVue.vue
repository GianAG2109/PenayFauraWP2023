<template>
	<div>
		<v-sheet class="bg-red-lighten-1 text-center d-flex flex-column">
			<h1 class="text-center pb-6 text-3xl md:text-4xl lg:text-5xl font-semibold text-red-600">Ubiquenos en Google Maps</h1>
		</v-sheet>


	</div>
	
	<div class="embed-container">
		   <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3900.7717973708945!2d-77.0123823856167!3d-12.127760446713475!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c7ffd84d618b%3A0x3a15b8cacbf1df9f!2sAv.+Alfredo+Benavides+2150%2C+Miraflores+15048!5e0!3m2!1ses-419!2spe!4v1552609669862" frameborder="0" allowfullscreen></iframe>
	</div>
</template>

<style>
.embed-container {
position: relative;
padding-bottom: 56.25%;
height: 0;
overflow: hidden;
}
.embed-container iframe {
position: absolute;
top:0;
left: 0;
width: 100%;
height: 100%;
}
</style>