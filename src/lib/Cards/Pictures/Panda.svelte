<div class="Panda">
	<div class="eye" id="eye2" />
	<div class="eye" />
	<div class="foot" id="foot2" />
	<div class="foot" />
	<div class="hand" />
	<div class="hand" id="hand2" />
	<div class="trunk" />
	<div class="ear" />
	<div class="ear" id="e2" />
	<div class="Head" />
	<div class="nose" />
</div>

<style>
	.Panda {
		position: relative;
		height: 130px;
		width: 120px;
	}

	.Head {
		height: 60px;
		width: 60px;
		border: solid black 1px;
		border-radius: 100%;
		background-color: white;
		position: absolute;
		left: 30px;
		top: 10px;
	}
	.ear {
		height: 30px;
		width: 30px;
		background-color: black;
		border-radius: 100%;
		position: absolute;
		left: 20px;
	}
	#e2 {
		left: 70px;
	}
	.trunk {
		height: 60px;
		width: 50px;
		border: solid 10px black;
		border-radius: 50%;
		background-color: white;
		position: absolute;
		left: 27px;
		top: 50px;
	}
	.hand {
		height: 30px;
		width: 30px;
		background: white;
		position: absolute;
		border-radius: 100%;
		z-index: 1;
		top: 60px;
		left: 18px;
		border: solid black 1px;
	}
	#hand2 {
		left: 76px;
	}
	.foot {
		height: 30px;
		width: 30px;
		background: black;
		position: absolute;
		border-radius: 100%;
		z-index: 1;
		top: 100px;
		left: 18px;
		border: solid black 1px;
	}
	#foot2 {
		left: 76px;
	}
</style>
