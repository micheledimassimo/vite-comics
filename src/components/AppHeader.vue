<script>
export default {
	data() {
		return { 
			navBarLinks: [
			{
                label: 'CHARACTERS',
                url: '#',
                active: false
            },
			{
                label: 'COMICS',
                url: '#',
                active: true
            },
			{
                label: 'MOVIES',
                url: '#',
                active: false
            },
			{
                label: 'TV',
                url: '#',
                active: false
            },
			{
                label: 'GAMES',
                url: '#',
                active: false
            },
			{
                label: 'COLLECTIBLES',
                url: '#',
                active: false
            },
			{
                label: 'VIDEOS',
                url: '#',
                active: false
            },
			{
                label: 'FANS',
                url: '#',
                active: false
            },
			{
                label: 'NEWS',
                url: '#',
                active: false
            }
			],
			headerLogo: './dc-logo.png'
		}
	}
}
</script>

<template>
	<header>
		<div class="header-container">
			<div class="logo-container">
				<img :src="headerLogo" alt="DC Comics">
			</div>
			<div>
				<nav>
					<ul>
						<li v-for="(link, index) in navBarLinks" :key="index">
							<a 
							:class="{
							'active': link.active
							}"
							href="link.url">
								{{ link.label }}
						</a>
						</li>
					</ul>
				</nav>
			</div>
		</div>
	</header>
</template>

<style lang="scss" scoped>
header {
	.header-container {
		display: flex;
		justify-content: space-between;
		align-items: center;
		max-width: 1200px;
		margin: 0 auto;
		padding: 10px;
		nav {
			ul {
				display: flex;
				list-style: none;
				li {
					padding: 10px;
					> a {
					text-decoration: none;
					font-weight: bold;
					color: #56566F;

					&:hover {
						color: #0282F9;
					}
					&.active {
						color: #0282F9;
					}
				}
				} 
				
			}
		}
	}
 
}


</style>
