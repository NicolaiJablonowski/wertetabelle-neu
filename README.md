<html>
	<head>
		<title>Kontrollstrukturen</title>
		<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<script>
			"use strict";

			// Programmiere hier calc
function clicked() {			
var i=1
var vAnzahl= document.getElementById("idZahl").value;
var vAusgabe = "";
var i2		
var i3
vAusgabe = vAusgabe + "<table border=1>";
vAusgabe = vAusgabe + "<tr><th>" + "x" + "</th><th>" + "x2" + "</th><th>"+"x3"+"</th></tr>";
while (i<=vAnzahl) {
i2= i*i
i3= i*i*i
vAusgabe= vAusgabe + "<tr><td>" +  i + "</td><td>" + i2 + "</td><td>" + i3 + "</td></tr>";
i= i+1;
}
document.getElementById("idOutput").innerHTML = vAusgabe;
}
</script>
	</head>
	<body>
		<h1>Kontrollstrukturen</h1>
		Eingabe: <input id="idZahl" type="text" value="10">
	<button onClick="clicked();">Berechne!</button>
		<div id="idOutput">Hier kommen die Zahlen</div>
	</body>
</html>
