<template>
	<div class="card-container">
		<div class="top">
			<div class="first">
				<p style="font-size: medium; font-weight: 400;">TOOK PAGEVIEWS</p>
				<p><span style="font-size: 50px;font-weight: 600;">$16.00</span>/month</p>
			</div>
			<div class="barre"></div>
		</div>
		<div class="middle">
			<span>Monthly Billing</span>
			<div> Toggle</div>
			<span>Yearly Billing</span>
			<span class="cover">25% <span class="disount">discount</span></span>
		</div>
		<div class="bottom">
			<div class="left">
				<div class="container">
					<Iconcheck info = "Unlimited websites"/>
					<Iconcheck info = "100% data ownership"/>
					<Iconcheck info = "Email reports"/>
				</div>
			</div>
			<div class="right">
				<button>Start my trial</button>
			</div>
		</div>
	</div>
</template>

<script>
import Iconcheck from "../components/Iconcheck.vue"

export default{
  components:{
    Iconcheck
  },

	data(){
		return{
			
		}
	}
}

</script>

<style scoped>
.card-container{
	background-color: #fff;
	padding: 20px 40px;
	height: 400px;
	width: 600px;
	display: grid;
	grid-template-rows: 45% 20% 35%;
	border-radius: 9px;
   box-shadow: 5px 4px 16px rgba(0,0,0,0.08);
}

.first {
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.bottom{
	padding-top: 20px;
	display: flex;
	border-top: 1px solid rgb(218, 207, 207);
}

.right{
	height: 100%;
	width: 50%;
	display: flex;
	justify-content: end;
	align-items: center;
}

.left{
	height: 100%;
	width: 50%;
	display: flex;
	flex-direction: column;
	justify-content: center;
}

button{
	background-color: hsl(227, 35%, 25%);
	height: 45px;
	width: 180px;
	color: #fff;
	display: flex;
	border-radius: 50px;
	display: flex;
	justify-content: center;
	align-items: center;
}

.middle{
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 0 20px;
	margin-left: 90px;
}

.cover{
	background-color:hsl(14, 92%, 95%);
	padding: 3px 8px;
	border-radius: 20px;
	color: hsl(15, 100%, 70%);
}


</style>