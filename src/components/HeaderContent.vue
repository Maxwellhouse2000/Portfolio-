<template>
	<div class="container header__content">
		<h1 class="header__content-title">
			<span>Hello, i'm Maqsud,</span> It's My Portfolio
		</h1>
		<div class="header__content-my-photo">
			<div class="header__content-my-photo-ram">
				<img src="@/assets/images/myphoto.jpg" alt="" />
			</div>
		</div>
	</div>
	<div class="header__content-my-descr">
		<p class="header__content-my-photo-text">
			my name is maqsud I'm 24 years old I want to become a front-end developer
		</p>
	</div>
</template>

<script>
export default {}
</script>

<style>
.header__content-my-photo-ram {
	width: 216px;
	height: 248px;
}
.header__content-my-photo-ram img {
	width: 216px;
	height: 248px;
}
.header__content-my-photo:hover {
	transform: scale(1.1) translateY(-5px);
}
.header__content-my-descr {
	margin-top: 10px;
	display: flex;
	justify-content: end;
	text-transform: capitalize;
}
.header__content-my-photo-text {
	font-size: 16px;
	font-weight: 600;
}

.header__content {
	display: flex;
	align-items: center;
	justify-content: space-between;
}
.header__content-title {
	display: flex;
	font-size: 80px;
	flex-direction: column;
}
.header__content-title span {
	text-transform: capitalize;
	font-size: medium;
}
.header__content-my-photo {
	padding: 40px;
	width: 100%;
	max-width: 320px;
	height: 348px;
	display: flex;
	align-items: center;
	border: 4px solid rgb(0, 0, 0);
	box-shadow: 0px 1px 3px 0px rgba(0, 0, 0, 0.3),
		0px 4px 4px 0px rgba(0, 0, 0, 0.25);
	background: rgba(0, 0, 0, 0);
	transition: 1s;
}

.header__content-my-photo-text {
	display: flex;
	margin-top: 10px;
	margin-bottom: 20px;
	padding: 20px;
}
.header__content-my-descr {
	border-bottom: 4px solid rgb(0, 0, 0);
	margin-bottom: 10px;
}

@media (max-width: 991.99px) {
	.header__content {
		min-height: 650px;
	}

	.header__content-title {
		margin-top: 100px;
		font-size: 60px;
		margin-bottom: 100px;
		text-align: center;
	}
	.header__content-my-descr {
		justify-content: center;
		text-align: center;
}
.header__content-my-photo-text {
	text-align: center;
}
}

@media (max-width: 767.99px) {
	.header__content-my-photo-ram img {
		max-width: 100%;
	}
	.header__content-my-photo-ram {
		max-width: 100%;
	}
	.header__content-my-photo {
		display: flex;
		align-items: center;
	}

	.header__content-my-descr {
		font-size: 40px;
		text-align: center;
		border-bottom: transparent;
	}
	.header__content-title {
		text-align: center;
	}
}

@media (max-width: 575.99px) {
}
</style>
