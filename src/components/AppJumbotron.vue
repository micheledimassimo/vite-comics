<script>




export default {
  data() {
    return { 
      
    }
  },

    
  }

</script>

<template>
	<div class="jumbo-container">
		<div>
			Current series
		</div>
	</div>
</template>

<style lang="scss" scoped>
	.jumbo-container {
		width: 100%;
		height: 400px;
		background-image: url("/jumbotron.jpg");
		background-position: top;
		
		> div {
			display: inline-block;
			background-color: #0282F9;
			padding: 20px;
			color: white;
			text-transform: uppercase;
			font-weight: bold;
			font-size: 1.25rem;
			position: absolute;
			top: 53%;
			left: 17%;
		}
	}
	
	
</style>
