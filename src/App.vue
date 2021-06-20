<template>
	<div>
		<Banner/>
		<Experience/>
		<Education/>
		<Gallery/>
		<Skills/>
		<Contact/>
		<a href="#Banner">
			<div class="scrollTop">
				<i class="fa fa-angle-up"></i>
			</div>
		</a>
	</div>
</template>

<script>
import Banner from './components/Banner.vue';
import Experience from './components/Experience.vue';
import Education from './components/Education.vue';
import Gallery from './components/Gallery.vue';
import Skills from './components/Skills.vue';
import Contact from './components/Contact.vue';

export default {
    name: 'App',
    components: {
		Banner,
		Education,
		Experience,
		Gallery,
		Skills,
		Contact
    }
}
</script>

<style>
@font-face {
    font-family: Sora-Regular;
    src: url(./assets/fonts/Sora-Regular.ttf);
}

@font-face {
    font-family: Sora-Bold;
    src: url(./assets/fonts/Sora-Bold.ttf);
}

* {
	text-transform: uppercase;
}

html {
	scroll-behavior: smooth;
}

body {
    margin: 0;
    text-align: center;
	background: url(assets/images/Portfolio.png);
	background-size: cover;
	background-position: top;
	background-repeat: repeat-y;
	background-color: #223;
	color: #F0F0F0;
}

body::-webkit-scrollbar {
  width: 1vw;
}
 
body::-webkit-scrollbar-track {
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
}
 
body::-webkit-scrollbar-thumb {
	border-radius: 1vw;
	background-color: darkgrey;
}

#app {
    font-family: Sora-Regular;
}
</style>
