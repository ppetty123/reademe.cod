<!DOCTYPE html>
<html>
<head>
	<title>Random Color Generator</title>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
	<h1>Random Color Generator</h1>
	<p>Click the button to generate a random color:</p>
	<button onclick="generateColor()">Generate</button>
	<div id="result" style="width: 100px; height: 100px;"></div>

	<script>
		function generateColor() {
			var letters = "0123456789ABCDEF";
			var color = "#";
			for (var i = 0; i < 6; i++) {
				color += letters[Math.floor(Math.random() * 16)];
			}
			document.getElementById("result").style.backgroundColor = color;
		}
	</script>
</body>
</html>
