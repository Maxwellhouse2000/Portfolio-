<template>
	<nav class="nav">
		<div class="container nav__content">
			<a href="#" class="nav__logo"> My Portfolio </a>
			<div class="nav__menu">
				<ul class="nav__list">
					<li v-for="(link, i) in links" :key="i">
						<a href="" class="nav__list-link">
							{{ link.name }}
						</a>
					</li>
				</ul>
				<div class="nav__menu-btn">
					<div class="nav__menu-btn-line"></div>
				</div>
			</div>
		</div>
	</nav>
</template>

<script>
export default {
	data() {
		return {
			links: [
				{ name: 'Home', to: 'Home' },
				{ name: 'About me', to: 'About me' },
				{ name: 'My works', to: 'My works' },
			],
		}
	},
}
</script>

<style>
.nav {
	padding: 30px 0;
	border-bottom: 6.28px solid rgb(0, 0, 0);
	margin-bottom: 50px;
}
.nav__logo {
	color: rgb(0, 0, 0);
	font-size: 24px;
}

.nav__content {
	display: flex;
	align-items: center;
	justify-content: space-between;
}

.nav__list {
	display: flex;
	gap: 20px;
}

.nav__list-link {
	transition: 1s;
	color: rgb(0, 0, 0);
	font-size: 16px;
}
.nav__list-link:hover {
	text-decoration: underline;
	transform: scale(1.1) translateY(-5px);
}
.nav__menu-btn {
	width: 25px;
	height: 25px;
	display: none;
	align-items: center;
	justify-content: center;
}

.nav__menu-btn-line {
	width: 100%;
	height: 2px;
	background-color: black;
	position: relative;
}
.nav__menu-btn:hover .nav__menu-btn-line {
	background-color: transparent;
}

.nav__menu-btn-line::before {
	content: '';
	width: 100%;
	height: 2px;
	background-color: black;
	position: absolute;
	top: -7px;
	transition: 0.5s;
}

.nav__menu-btn:hover .nav__menu-btn-line::before {
	top: 0;
	transform: rotate(45deg);
}

.nav__menu-btn:hover .nav__menu-btn-line::after {
	top: 0;
	transform: rotate(-45deg);
}

.nav__menu-btn-line::after {
	content: '';
	width: 100%;
	height: 2px;
	background-color: black;
	position: absolute;
	top: 7px;
	transition: 0.5s;
}

.nav__menu {
	display: flex;
	align-items: center;
}

@media (max-width: 991.99px) {
	.nav {
		border-bottom: transparent;
	}
	.nav__list-link {
		font-size: 20px;
		margin-left: 54px;
	}

	.header__content {
		min-height: 650px;
		flex-direction: column;
	}
}

@media (max-width: 767.99px) {
	.nav__logo {
		font-size: 32px;
	}

	.nav {
		position: relative;
	}

	.header__content-title {
		font-size: 32px;
		text-align: center;
	}
	.nav__list {
		position: absolute;
		flex-direction: column;
		
		top: -300px;
		padding: 15px;
		gap: 10px;
		right: 0;
		transition: 0.5s;
	}

	.nav__menu:hover .nav__list {
		top: 100%;
	}

	.nav__list-link {
		margin-left: 0;
	}

	.nav__menu-btn {
		display: flex;
	}
}

@media (max-width: 575.99px) {
}
</style>
