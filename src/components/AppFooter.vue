<script>
export default {
	data() {
		return { 
			
			footerLogos: [ 
				{
				logoImage: 'footer-facebook.png',
				url: '#',
				logoTitle: 'facebook'
				},
				{
				logoImage: 'footer-twitter.png',
				url: '#',
				logoTitle: 'twitter'
				},
				{
				logoImage: 'footer-youtube.png',
				url: '#',
				logoTitle: 'youtube'
				},
				{
				logoImage: 'footer-pinterest.png',
				url: '#',
				logoTitle: 'pinterest'
				},
				{
				logoImage: 'footer-periscope.png',
				url: '#',
				logoTitle: 'periscope'
				}
			
				
			]
		}
	}
}
</script>

<template>
	<footer>
		<div class="footer-container">
			<div >
				<button class="my-btn">
					<a href="#">
						Sign-up now!
					</a>
				</button>
			</div>
			<div>
				<nav>
					<ul>
						<li>
							<a class="follow-us-link" href="#">
								follow us
							</a>
						</li>
						<li v-for="(logo, index) in footerLogos" :key="index">
							<a 
							:href="logo.url">
								<img :src="logo.logoImage" :alt="logo.logoTitle">
						</a>
						</li>
					</ul>
				</nav>
			</div>
		</div>
	</footer>
</template>

<style lang="scss" scoped>
footer {
	background-color: #303030;
	.footer-container {
		display: flex;
		justify-content: space-between;
		align-items: center;
		max-width: 1200px;
		margin: 0 auto;
		padding: 10px;
		.my-btn {
			background-color: #303030;
			border: 1px solid #0282F9;
			padding: 10px;
			> a {
				text-decoration: none;
				color: white;
				text-transform: uppercase;
			}
		}
		nav {
			ul {
				display: flex;
				list-style: none;
				align-items: center;
				li {
					padding: 10px;
					> a {
					text-decoration: none;
					text-transform: uppercase;
					color: #56566F;

					&:hover {
						background-color: #0282F9;
						}
					
					}
				} 
				
			}
		}
	}
 
}


</style>
