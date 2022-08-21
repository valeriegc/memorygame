<article class="container">
	<div class="head">
		<div class="ear leftEar" />
		<div class="ear rightEar" />
		<div class="eye leftEye" />
		<div class="eye rightEye" />
		<div class="nose">
			<div class="nostril leftNostril" />
			<div class="nostril rightNostril" />
		</div>
	</div>
	<div class="body" />
</article>

<style>
	.container {
		margin-top: 35px;
		position: relative;
	}
	div {
		background: repeating-linear-gradient(0deg, #000000, black 5px, white 5px, #ffffff 10px);
		border-radius: 50%;
		border: 4px solid black;
	}
	.body {
		width: 60px;
		height: 85px;
	}
	.head {
		width: 40px;
		height: 70px;
		position: absolute;
		top: -25px;
		left: 10px;
		background: white;
	}
	.ear {
		position: absolute;
		width: 10px;
		height: 25px;
		background: rgb(7, 4, 3);
		top: -17px;
	}
	.leftEar {
		right: -6px;
	}
	.rightEar {
		left: -6px;
	}
	.eye {
		position: absolute;
		width: 3px;
		height: 8px;
		background: black;
		border: white 4px solid;
		box-shadow: 0 0 0 4px black;
		top: 20px;
	}
	.leftEye {
		left: 5px;
	}
	.rightEye {
		right: 5px;
	}
	.nose {
		position: absolute;
		width: 40px;
		height: 30px;
		background: grey;
		top: 50px;
		left: -4px;
	}
	.nostril {
		position: absolute;
		width: 5px;
		height: 7px;
		background: rgb(55, 55, 55);
		top: 7px;
	}
	.leftNostril {
		left: 4px;
	}
	.rightNostril {
		right: 4px;
	}
</style>
