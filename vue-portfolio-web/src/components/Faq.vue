<template>
  <div class="hello">
    <div class="item">
      <div class="bar">
        <h2>SmartCell Repair</h2>
        <i></i>
      </div>
      <div class="project_img"></div>
    </div>
    <div class="item">
      <div class="bar">
        <h2>SmartCell Repair</h2>
        <i></i>
      </div>
      <div class="project_img two">

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'faq'
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped >
*,
*:before,
*:after
	padding: 0
	margin: 0
	box-sizing: border-box
//general styles 
h2
	text-align: center
	text-transform: uppercase
	font-size: 10px
	font-weight: 700
	line-height: 24px
	color: #8a8a8a
	letter-spacing: -0.5px
.hello
	background: #2a2a2a
	min-height: 100vh
	display: flex
	flex-wrap: wrap
	justify-content: space-around
	align-items: center
	font-family: MontSerrat,Tahoma,arial
.item	
	flex-basis: 400px
	max-width: 500px
  min-width: 90%
	background: #f3f3f3
	//padding: 1.2rem
	box-shadow: 8px 8px 0 rgba(#000,.16)	
	position: relative
	.bar
		height: 24px
		background: rgba(#ddd,0.9)
		color: #6a6a6a
		width: 100%
i:before,
i:after
	content: ''
	top: 0
i	,
i:before,
i:after
	height: 12px
	width: 12px
	display: inline-block
	border-radius: 50%
	position: absolute

i
	background: #ff5f57
	top: 6px
	left: 10px
	&:after
		left: 32px
		background: green
i:before
	background: yellow
	left: 16px
.project_img
	max-height: 50%
	height: 300px
	background: linear-gradient(rgba(#000,0.3),rgba(#000, 0.6)),url('../assets/Screenshot-2018-5-15 Smart Cell Repair Iphone , samsung laptop repair.png') center center no-repeat

	background-size: cover
.two
	background: linear-gradient(rgba(#000,0.2),rgba(#000, 0.6)),url('../assets/smartcellrepairt.jpg') center center no-repeat
	background-size: cover
</style>
