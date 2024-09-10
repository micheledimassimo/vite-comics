<script>




export default {
  data() {
    return { 
		mainLinks: [
			{
				image: './buy-comics-digital-comics.png',
				text: 'DIGITAL COMICS',
				link: '#'
			},
			{
				image: './buy-comics-merchandise.png',
				text: 'DC MERCHANDISE',
				link: '#'
			},
			{
				image: './buy-comics-subscriptions.png',
				text: 'SUBSCRIPTION',
				link: '#'
			},
			{
				image: './buy-comics-shop-locator.png',
				text: 'COMIC SHOP LOCATOR',
				link: '#'
			},
			{
				image: './buy-dc-power-visa.svg',
				text: 'DC POWER VISA',
				link: '#'
			},
		]
    }
  }
  
  }

</script>

<template>
  
	<div class="my-bg-blue">
		<div class="my-container">
		<div class="my-row">
			<div v-for="(link, index) in mainLinks" :key="index" 
			class="my-col-1-5">
				<div 
				class="my-row">
					<a :href="link.link">
						<img :src="link.image" :alt="link.text">
						<p>
							{{ link.text }}
						</p>
					</a>

				</div>
			</div>
		</div>
	</div>
	</div>
    
  
</template>

<style lang="scss" scoped>

	.my-container {
		max-width: 1200px;
		margin: 0 auto;
		.my-row {
			display: flex;
			justify-content: space-between;
			align-items: center;
			> .my-col-1-5 {
				width: calc((100% / 5) - 25px);
				margin-left: 10px;
				padding: 20px 0;
				


				> .my-row > a {
					text-decoration: none;
					color: white;
					font-size: 0.75rem;
					
					display: flex;
					align-items: center;
					
					> img {
						width: 50px;
						object-fit: cover;
						margin-right: 5px;
						
					}
					
				}
			}
		}
	}
	.my-bg-blue {
		background-color: #0282F9;
	}
</style>
