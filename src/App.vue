<template>
	<div class="wrapper">
		<header class="header">
			<NavBar />
			<HeaderContent />
		</header>
		<SkillsSection />
		<PortfolioSection />
		<Footer/>
	</div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeaderContent from './components/HeaderContent.vue'
import SkillsSection from './components/SkillsSection.vue'
import PortfolioSection from './components/PortfolioSection.vue'
import Footer from './components/Footer.vue'

export default {
	components: {
		NavBar,
		HeaderContent,
		SkillsSection,
		PortfolioSection,
		Footer
	},
}
</script>

<style>
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Montserrat';
	background: white;
}

a {
	text-decoration: none;
}
li {
	list-style: none;
}
input,
button {
	background: none;
	outline: none;
	border: none;
	transition: 0.5s;
}

.container {
	width: 100%;
	max-width: 1140px;
	padding: 0 15px;
	margin: 0 auto;
}
.wrapper{
	/* overflow-y: hidden; */
}
</style>
