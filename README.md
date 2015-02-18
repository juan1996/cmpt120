<!DOCTYPE html>
<html>
<!-- Juan Diaz Febuary 18,2015 Project 2 -->
<head>
	<title>My First Game</title>
<style>
	body {background-color:pink}
	<p><br>The Lost One</p>
	</style>
	<script>

var score = 0;
var lNV = false;
var lSV = false;
var lEV = false;
var lWV = false;

function scoreFunction()
{
	var scorefield = document.getElementById("myText");
	scorefield.value = score;
	scorefield.style.color="green";
}

function northDirection()  {
var msg = "Ran into a dark ally.";
	if (lNV == false) {
		lNV = true
		score +=5
	}
	scoreFunction();
	alert(msg);
}

function southDirection()  {
var msg = "Someone is following you.";
	if (lSV == false) {
		lSV = true
		score +=5
	}
	scoreFunction();
	alert(msg);
}

function eastDirection()  {
var msg = "You are about to lose him.";
	if (lEV == false){
		lEV = true
		score +=5
	}
	scoreFunction();
	alert(msg);
}

function westDirection()  {
var msg = "You go out the ally.";
	if (lWV == false) {
		lWV = true
		score +=5
	}
	scoreFunction();
	alert(msg);
}


</script>
</head>
<body>
<h1>The Lost One</h1>

	&nbsp;&nbsp;&nbsp;&nbsp; <input type="button" value="North" onClick="northDirection()">
	<br>
	<br>
	<input type="button" value="West" onClick="westDirection()">
	<input type="button" value="East" onClick="eastDirection()">
	<br>
	<br>

	&nbsp;&nbsp;&nbsp;&nbsp;<input type="button" value="South" onClick="southDirection()">

<p></p>
<br>
Score: <input type="text" id="myText" size="7">
<br><br><a href="mailto:juan.diaz1@marist">My email</a>
</body>
</html>



