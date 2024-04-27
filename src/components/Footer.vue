<template>
	<footer class="footer">
		<div class="container footer__content">
			<ul class="footer__content-list-2">
				<li v-for="(contact, i) in contact" :key="i">
					<a class="footer__content-list-link" :href="contact.link">
						<img :src="contact.img" alt="" />
						{{ contact.link }}
					</a>
				</li>
			</ul>
			
		</div>
	</footer>
</template>

<script>
export default {
	data() {
		return {
			contact: [
				{
					link: 'Tel:+998 90 912 93 70',
					img: require('@/assets/icons/phone.svg'),
				},
				{
					link: 'Mailto:maxsudulugxojaev@gmail.com',

					img: require('@/assets/icons/email.svg'),
				},
			],
		}
	},
}
</script>

<style>
.footer {
	margin-top: 50px;
	padding: 50px 0;
	border-top: 6.28px solid rgb(0, 0, 0);
}
.footer__content {
	display: flex;
	align-items: center;
	justify-content: space-between;
}
.footer__content-list {
	display: flex;
	gap: 10px;
}
.footer__content-list-link {
	display: flex;
	align-items: center;
	color: rgb(0, 0, 0);
	font-size: 16px;
	gap: 10px;
}
.footer__content-list-link img {
	width: 2%;
}
.footer__content-list-link:hover {
	text-decoration: underline;
	transform: scale(1.1) translateY(-5px);
}
.footer__content-list-link {
	transition: 1s;
}
.footer__content-list-2 {
	display: flex;
	flex-direction: column;
	gap: 20px;
}


@media (max-width:767.99px) {
    
    .footer__content {
        display: flex;
        gap: 20px;
        flex-wrap: wrap;
    }
	.footer {
	margin-top: 50px;
	padding: 50px 0;
	border-top: transparent;
}
}

@media (max-width:575.99px) {
	.footer__content-list-link{
		font-size: 12px;
	}
}
</style>
