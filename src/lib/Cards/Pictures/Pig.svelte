<article class="wrap">
	<div class="ears" />
	<div class="ears" id="earRight" />
	<div class="head">
		<div class="eyes" />
		<div class="eyes" id="eyeRight" />
		<div class="nose">
			<div class="nostrils" />
			<div class="nostrils" id="nostrilRight" />
		</div>
	</div>
</article>

<style>
	div {
		background-color: rgb(255, 197, 206);
		border: solid black 4px;
	}
	.wrap {
		height: 100%;
		width: 100%;
		display: flex;
		align-items: center;
		justify-content: center;
		position: relative;
	}
	.head {
		height: 80px;
		width: 90px;
		border-radius: 50%;
		z-index: 1;
		position: relative;
	}
	.ears {
		border: solid black 4px;
		height: 50px;
		width: 50px;
		border-top-right-radius: 50px;
		border-bottom-left-radius: 50px;
		position: absolute;
		top: 30px;
		background-color: rgb(255, 197, 206);
		left: 20px;
	}
	#earRight {
		left: 60px;
		transform: rotate(90deg);
	}
	.nose {
		height: 20px;
		width: 30px;
		position: absolute;
		left: 26px;
		top: 35px;
		border-radius: 50%;
	}
	.nostrils {
		height: 0px;
		width: 0px;
		border-radius: 50%;
		background-color: black;
		position: absolute;
		left: 5px;
		top: 3px;
	}
	#nostrilRight {
		left: 17px;
	}
	.eyes {
		width: 10px;
		height: 10px;
		border: white solid 5px;
		background-color: black;
		border-radius: 100%;
		left: 10px;
		position: absolute;
		top: 20px;
	}
	#eyeRight {
		left: 60px;
	}
</style>
