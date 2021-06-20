<template>
	<div id="Banner" class="Compartment">
		<Navigation />		
		<div class="name-card">
			<img src="@/assets/images/profile.png" class="profileImg"/>
			<div>Suhib Irsheidat</div>
			<div>UI/UX &amp; Front End Developer</div>
		</div>
	</div>
</template>

<script>
import Navigation from "./Navigation.vue";

export default {
	name: 'Banner',
	components: {
		Navigation
	},
	props: {
	}
}
</script>

<style>
.Compartment{
	width: 98vw;
	height: 100vh;
	margin: 0;
	position: relative;
	overflow-x: hidden;
}

.profileImg{
	width: 20vw;
	height: 20vw;
	border-radius: 50%;
}

.name-card{
	width: 75vw;
	height: 20vw;
	text-align: left;
	margin: 0;
	margin-top: calc(50vh - 14vw);
	margin-left: 18vw;
	position: relative
}

.name-card div:nth-child(2){
	position: absolute;
	top: 6.5vw;
	left: 22vw;
	letter-spacing: 0.35vw;
	color: #f0f0f0;
	font-size: 3.5vw;
	font-family: Sora-Bold;
}

.name-card div:nth-child(3){
	position: absolute;
	top: 11.5vw;
	left: 22vw;
	letter-spacing: 0.35vw;
	color: #f0f0f0;
	font-size: 1.25vw;
	font-family: Sora-Regular;
}

.scrollTop{
	width: 4vw;
	height: 4vw;
	background: #40A4FF;
	font-size: 3vw;
	position: fixed;
	bottom: 2vw;
	right: 2vw;
	border-radius: 50%;
	box-shadow: 0 1vw 2vw #0004;
}
</style>
