<template>
	<!-- Hero en home -->
	<div class="w3-container w3-center w3-padding-24">
		<h2>Los mejores productos alimenticios para su desayuno</h2>
		<p>¡Bienvenidos a nuestro pequeño negocio de productos de panadería! Ofrecemos una gran variedad de delicias, incluyendo hojaldras, arepas y dedos de queso, todos hechos con ingredientes frescos y de alta calidad.</p>
		<p>Nuestros productos son ideales para disfrutar en casa o para compartir con amigos y familiares en cualquier ocasión. También ofrecemos diferentes sabores y rellenos para satisfacer todos los gustos. Además, como pequeño negocio local, nos esforzamos por ofrecer precios competitivos y un servicio personalizado y amigable. ¡Visítanos y prueba nuestros deliciosos productos!</p>
	</div>

	<!-- contenido -->
	<div class="w3-row-padding w3-container s12 w3-padding-32">
		<div class="w3-col w3-cell m4 s12">
			<img src="../img/hojaldra.jpg" class="w3-image w3-round" alt="">
			<div class="w3-container">
				<h3>Deliciosas hojaldras con receta exclusiva</h3>
				<p>¡Las hojaldras de harina son una delicia crujiente y deliciosa! Son un pan tradicional que se caracteriza por su textura hojaldrada y suave sabor a mantequilla.</p>
			</div>
		</div>
		<div class="w3-col w3-cell m4 s12">
			<img src="../img/arepa.jpg" class="w3-image w3-round" alt="">
			<div class="w3-container">
				<h3>Arepas caseras con queso, recien hechecitas</h3>
				<p>¡Las arepas son deliciosas y versátiles! Son un plato tradicional de la gastronomía latinoamericana que puedes disfrutar en cualquier momento del día.</p>
			</div>
		</div>
		<div class="w3-col w3-cell m4 s12">
			<img src="../img/dedo.jpg" class="w3-image w3-round" alt="">
			<div class="w3-container">
				<h3>Dedos de queso deliciosos</h3>
				<p>¡Los dedos de queso son una delicia irresistible! Son una botana crujiente y sabrosa que combina la suavidad del queso con la textura dorada y crujiente del pan rallado.</p>
			</div>
		</div>
	</div>

	<PageFooter/>
</template>

<script>
// @ is an alias to /src
import PageFooter from '@/components/PageFooter.vue';

export default {
  name: 'HomeView',
  components: {
    PageFooter
  }
}
</script>
