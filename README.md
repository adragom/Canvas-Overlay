# Canvas-Overlay
Background Image with a color overlay using canvas

<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Background Image</title>
	<style>
		
		body,html{
			padding: 0;
			margin: 0;
			font-family: monospace;
			font-size: 120%;
			letter-spacing: 1.5px;
			background-color: #262626;
			
		}
		
		header{
			text-align: center;
			text-decoration: underline;
			padding: 20px;
			
		}
		
		
		article{
			height: 490px;
			background: url("https://upload.wikimedia.org/wikipedia/commons/e/e2/OrteliusWorldMap1570.jpg");
			background-repeat: no-repeat;
			background-position: center;
		    background-size: cover;
			opacity: 1;
			
			
		}
	
		canvas{
			width: 100%;
			height: 490px;
			opacity: 0.9;
		}
	</style>
</head>
<body>

<header>
	<h1>Background Image with overlay color using Canvas</h1>
</header>

<hr>

<article>
	<canvas id="color"></canvas>
		
</article>
	
	<script>
	window.onload = init();	
		
	var canvas, ctx;
		function init(){
			canvas = document.getElementById('color');
			ctx = canvas.getContext('2d');
			
			ctx.save();
			ctx.fillStyle='#00833D';     //  #00843D   // 118846
			ctx.fillRect(0,0,490,490);
			ctx.restore();		
		}		
	</script>
	<hr>
</body>
</html>
