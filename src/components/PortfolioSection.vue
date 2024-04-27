<template>
	<section class="portfolio">
		<h1 class="skills__title portfolio__title">My Portfolio</h1>
		<div class="container portfolio__content">
			<div
				class="portfolio__content-item"
				v-for="(card, index) in card"
				:key="index"
			>
				<img :src="card.img" alt="" />
				<div class="portfolio__content-item-info">
					<h2 class="portfolio__content-title">{{ card.title }}</h2>
					<button class="portfolio__content-btn">
						<a
							target="_blank"
							:href="card.link"
							class="portfolio__content-btn-link"
							>{{ card.button }}</a
						>
					</button>
				</div>
				<p class="portfolio__content-descr">{{ card.descr }}</p>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	data() {
		return {
			card: [
				{
					img: require('@/assets/images/aboutme.png'),
					title: 'About me',
					descr: 'My first project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/Vue-js/'
				},
				{
					img: require('@/assets/images/silverhouse.png'),
					title: 'Silver House',
					descr: 'My second project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/Silver-House/'
				},
				{
					img: require('@/assets/images/gotrip.png'),
					title: 'GoTrip',
					descr: 'My third project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/GoTrip/'
				},
				{
					img: require('@/assets/images/news.png'),
					title: 'The News Web',
					descr: 'My four project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/news/'
				},
				{
					img: require('@/assets/images/nike.png'),
					title: 'Nike',
					descr: 'My five project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/nike/'
				},
				{
					img: require('@/assets/images/grayson.png'),
					title: 'Grayson',
					descr: 'My six project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/grayson/'
				},
				{
					img: require('@/assets/images/totembo.png'),
					title: 'Totembo',
					descr: 'My seven project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/Totembo/'
				},
				{
					img: require('@/assets/images/market.png'),
					title: 'Boulevard Market',
					descr: 'My eight project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/Boulevard-market/'
				},
				{
					img: require('@/assets/images/expo.png'),
					title: 'ExpoForum',
					descr: 'My nine project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/ExpoForum/'
				},
				{
					img: require('@/assets/images/film.png'),
					title: 'CinePhile',
					descr: 'My ten project',
					button: 'Go to WebSite',
					link: 'https://maxwellhouse2000.github.io/-cinephile/'
				},
			],
		}
	},
}
</script>

<style>
.portfolio__content-item-info {
	display: flex;
	justify-content: space-between;
}
.portfolio__content {
	display: grid;
	grid-template-columns: repeat(2, 1fr);
	gap: 20px;
}
.portfolio__content-item {
	padding: 50px;
	justify-items: center;
	border: 6.28px solid rgb(0, 0, 0);
}
.portfolio__content-item img {
	width: 100%;
	border: 4px solid rgb(0, 0, 0);
	box-shadow: 0px 1px 3px 0px rgba(0, 0, 0, 0.3),
		0px 4px 4px 0px rgba(0, 0, 0, 0.25);
	background: rgba(0, 0, 0, 0);

	transition: 1s;
}
.portfolio__content-item img:hover {
	transform: scale(1.1) translateY(-5px);
}

.portfolio__content-title {
	margin-top: 20px;
}
.portfolio__content-descr {
	margin-top: 10px;
}
.portfolio__content-btn {
	margin-top: 20px;
	display: flex;
	transition: 1s;
}
.portfolio__content-btn:hover {
	transform: scale(1.1) translateY(-5px);
}
.portfolio__content-btn-link {
	color: #ffffff;
	padding: 10px;
	background-color: black;
	transition: 1s;
}
.portfolio__content-btn-link:hover {
	background: red;
}
@media (max-width:1199.99px) {

   
   
    
}

@media (max-width:991.99px) {
  
    
    
   
    .portfolio__content {
		display: flex;
		flex-direction: column;
    }
}

@media (max-width:767.99px) {
   

    .portfolio__content-title {
        font-size: 32px;
        text-align: center;
    }
    .portfolio__content-item-info {
		text-align: center;
		align-items: center;
        flex-direction: column;
    }
    .portfolio__content-descr {
	text-align: center;
}
}

@media (max-width:575.99px) {}
</style>
