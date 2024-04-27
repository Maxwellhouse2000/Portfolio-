<template>
	<main class="main">
		<section class="skills">
			<h1 class="skills__title">My Skills</h1>
			<div class="container skills__content">
				<div class="skills__content-item">
					<ul class="skills__content-item-list">
						<h2 class="skills__content-title">what i know</h2>
						<li>
							<p class="skills__content-item-text">"reinstall windows"</p>
						</li>
						<li>
							<p class="skills__content-item-text">"programming"</p>
						</li>
						<li>
							<p class="skills__content-item-text">"analise football"</p>
						</li>
					</ul>
				</div>
				<div class="skills__content-item">
					<ul class="skills__content-item-list">
						<h2 class="skills__content-title-2">what i dont know</h2>
						<li>
							<p class="skills__content-item-text-2">"cooking"</p>
						</li>
						<li>
							<p class="skills__content-item-text-2">
								"drive car"
							</p>
						</li>
						<li>
							<p class="skills__content-item-text-2">"fishing"</p>
						</li>
					</ul>
				</div>
			</div>
		</section>
	</main>
</template>

<script>
export default {}
</script>

<style>
.skills__title {
	text-align: center;
	font-size: 50px;
	margin-bottom: 50px;
}

.skills__content {
	margin-top: 10px;
	display: flex;
	align-items: center;
	justify-content: space-between;
}
.skills__content-item {
	box-sizing: border-box;
	border-top: 3px solid rgb(0, 0, 0);
	border-bottom: 3px solid rgb(0, 0, 0);
	border-left: 3px solid rgb(0, 0, 0);
	border-right: 3px solid rgb(0, 0, 0);
	display: flex;
	padding: 10px;
	margin-bottom: 50px;
	transition: 1s;
}
.skills__content-item:hover {
	transform: scale(1.1) translateY(-5px);
}
.skills__content-item-list {
	display: flex;
	flex-direction: column;
}
.skills__content-item-text:hover {
	color: rgb(255, 255, 255);
	background: rgba(31, 110, 31, 0.827);
}
.skills__content-title {
	text-transform: capitalize;
	color: rgb(0, 0, 0);
	font-size: 36px;
	font-weight: 700;
	line-height: 46px;
}
.skills__content-title:hover {
	color: rgba(31, 110, 31, 0.827);
}
.skills__content-item-text {
	text-transform: capitalize;
	color: rgb(0, 0, 0);
	font-size: 24px;
	font-weight: 500;
	line-height: 31px;
}
.skills__content-title-2 {
	text-transform: capitalize;
	color: rgb(0, 0, 0);
	font-size: 36px;
	font-weight: 700;
	line-height: 46px;
}
.skills__content-item-text-2 {
	text-transform: capitalize;
	color: rgb(0, 0, 0);
	font-size: 24px;
	font-weight: 500;
	line-height: 31px;
}
.skills__content-title-2:hover {
	color: rgb(130, 24, 24);
	
}
.skills__content-item-text-2:hover {
	color: rgb(255, 255, 255);
	background: rgb(130, 24, 24);
}
@media (max-width:1199.99px) {

    .skills__content {
        gap: 30px;
    }
    
   
    
}

@media (max-width:991.99px) {
   
    
    .header__content{
        min-height: 650px;
		flex-direction: column;
    }
   
    .skills__content {
        justify-content: center;
		flex-direction: column;
    }
}

@media (max-width:767.99px) {
   

    .skills__content-title {
        font-size: 32px;
        text-align: center;
    }
   

    
    .skills__title {
        
        font-size: 50px;
    }
   
    
}

@media (max-width:575.99px) {}
	

</style>
