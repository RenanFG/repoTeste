# ***repoTeste***
***Repositório***

`
<!doctype html>
<html lang=“pt-br”>
	<head>
		<title>Curso de Javascript</title>
		<meta charset=“UTF-8”>
		<script>
		
			function relogio(){
				var data=new Date();
				var hor=data.getHours();
				var min=data.getMinutes();
				var seg=data.getSeconds();
				
				if(hor < 10){
					hor="0"+hor;
				}
				if(min < 10){
					min="0"+min;
				}
				if(seg < 10){
					seg="0"+seg;
				}
				
				var horas=hor + ":" + min + ":" + seg;
				
				document.getElementById("rel").value=horas;
			}

			var timer=setInterval(relogio,1000);

		</script>
	</head>
	<body>
		<input type="text" id="rel">
	</body>
</html>
`
