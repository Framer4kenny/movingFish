# movingFish
1. call jquery
2. start jquery (document).ready = doc + ready + function
3. id + click + function

```
1.
<!-- <script src="http://code.jquery.com/jquery-latest.min.js"></script> -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
```

```
2.
		$(document).ready(function(){
			var $fish = $("#fishImage");
```

```
3.
			$("#fishBT").click(function(){
				$fish.animate({
					left: "750px"
				}, 1000);
```

```
<!DOCTYPE html>
<html>
<head>
	<title>movingFish</title>
	<!-- <script src="http://code.jquery.com/jquery-latest.min.js"></script> -->
	<style type="text/css">
		#fishImage {
			position: absolute;
			padding: 30px;
			width: 150px;
		}
		#nav {
			text-align: center;
			position: relative;
			margin-top: 150px;

		}
	</style>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
	<script>
		$(document).ready(function(){
			var $fish = $("#fishImage");

			$("#fishBT").click(function(){
				$fish.animate({
					left: "750px"
				}, 1000);
			});
		})
	</script>

</head>

<body>
<div>
<img src = "./fish.png" id="fishImage">
</div>
<br>
<div id="nav">
<button id="fishBT">이동하기</button>

</div>


</body>
</html>
```
