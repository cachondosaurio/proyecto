<!DOCTYPE html>
<!-- saved from url=(0169)file:///C:\Users\mane_\OneDrive\Escritorio\Último Semestre\Fundamentos de base de datos\Cuarto Parcial\Proyecto 4to parcial\Aplicacion Web.html?Estado=0#-->

<html lang="en"><head><meta http-equiv=refresh content=120>
	<title>PAWS & MUNCHIES</title>
	<link rel="stylesheet" href="style.css">
</head>

<body>
	<img src="itcelaya logo.png" class="imagen" alt="">

	<div id="Ingresar">
		<h1 class="Titulo">"PAWS & MUNCHIES"</h1>
		<h4 class="Subtitulo">Fundamentos de Bases de datos e Internet de las cosas
  
		Usuario: <span id="user"></span>
		Estado: <span id="edo"></span></h4>
		
		<form class="Seleccion" action="file:///C:\Users\mane_\OneDrive\Escritorio\Último Semestre\Fundamentos de base de datos\Cuarto Parcial\Proyecto 4to parcial\Aplicacion Web.html?Estado=0#">

		<label class="Accion" for="ingresaAccion"> Compuerta  </label>
		<select class="CSelect" name="Estado" id="ingresaAccion">
		<option class="Abrir" value="0"> Abrir </option>
		<option class="Cerrar" value="1"> Cerrar</option>
		</select>
		<br><br/>
		</form>

		<button class="ComVerde" id="verde">Comedero de aves</button>
		<button class="ComAzul" id="azul">Comedero de ardillas</button>
		<button class="ComRojo" id="rojo">Comedero de perros</button>
		<button class="ComAmarillo" id="amarillo">Comedero de tlacuaches</button>
		
		<h5 class="Info">Información</h5>

		<div class="ventanaverde" id="infoverde">
			
			<div id="cerrarverde"><a href="javascript:cerrarv()"><img src="cerrar.png"></a></div>
				INFORMACIÓN DE AVES
		
				<! - Informacion obtenida de https://www.revista.unam.mx/vol.3/num1/sabias1/que.html ->
				<p class="textoaves">
					Las aves son animales vertebrados, es decir, que poseen una columna vertebral, al igual que un gato o un conejo. Mantienen la temperatura corporal constante al igual que nosotros. Por ello se conocen como animales endotérmicos.
					Las aves se caracterizan por tener plumas, con las que pueden volar y protegerse del ambiente.<br><br>			
					Además, las aves se dividen en aves canoras y de ornato, mejor conocidas como pájaros, por su gran variedad de cantos y notas musicales. Las aves sólo emiten sonido y graznidos. En México se tienen registradas 1060 especies de aves, distribuidas en diferentes ambientes como bosques tropicales y templados, y zonas áridas y urbanas, entre otros.
				</p><img src="House sparrow.png" class="fotoaves"><br><br>

				Estado de los comederos
			
			</div>

		<button class="Verde"><a href="javascript:infoave()">Info Aves</a></button>
		<script>
			function infoave(){
				document.getElementById("infoverde").style.display="block";
			}
			function cerrarv(){
				document.getElementById("infoverde").style.display="none";
			}

		</script>


	<div class="ventanaazul" id="infoazul">
				
		<div id="cerrarazul"><a href="javascript:cerrara()"><img src="cerrar.png"></a></div>
			INFORMACIÓN DE ARDILLAS

			<! - Informacion obtenida de https://animalia.bio/es/mexican-gray-squirrel ->
			<p class="textoardillas">
				La ardilla gris mexicana (Sciurus aureogaster), conocida en México simplemente como ardilla gris, y también como ardilla arborícola o ardilla vientre rojo, 
				es una especie de roedor esciuromorfo de la familia Sciuridae (ardillas y parientes, ).
				Es una ardilla arborícola originaria de Guatemala y del este y sur de México, y ha sido introducida en algunas regiones de Florida (Estados Unidos) y de Argentina.<br><br> 
				En México habita en 23 estados (las entidades donde no se ha registrado su presencia son: Baja California, Baja California Sur, Sonora, Chihuahua, Coahuila, Sinaloa, Durango, Quintana Roo y Yucatán). 
				Su pelaje es gris y blanco, rojizo en el abdomen; existen individuos negros. Mide entre 42 y 55 cm con una cola de 20 a 30 cm de longitud. Orejas y ojos pequeños. Sus dientes son fuertes y los usa para abrir nueces.
			</p><img src="Ardilla.png" class="fotoardillas"><br><br>

			Estado de los comederos
		
		</div>
		<button class="Azul"><a href="javascript:infoardillas()">Info Ardillas</a></button>
		<script>
			function infoardillas(){
				document.getElementById("infoazul").style.display="block";
			}
			function cerrara(){
				document.getElementById("infoazul").style.display="none";
			}

		</script>


		<div class="ventanaroja" id="inforojo">
					
		<div id="cerrarrojo"><a href="javascript:cerrarr()"><img src="cerrar.png"></a></div>
			INFORMACIÓN DE PERROS

			<! - Informacion obtenida de https://www.nationalgeographicla.com/animales/perro-domestico ->
			<p class="textoperros">
				El término “perro doméstico” se refiere a cualquiera de los cientos de razas de perros que hay en el mundo hoy en día. 
				Si bien estos animales varían drásticamente en cuanto a su apariencia, todos los perros, desde el chihuahua hasta el gran danés, son miembros de la misma especie, Canis familiaris. 
				Esto separa a los perros domésticos de los caninos salvajes, como coyotes, zorros y lobos. <br><br>
				Los perros domésticos se mantienen principalmente como mascotas, aunque muchas razas son capaces de sobrevivir por sí mismas, ya sea en un bosque o en las calles de una ciudad. 
				Según un estudio realizado en 2016, un tercio de todos los hogares del mundo tienen un perro. Esto convierte al perro doméstico en la mascota más popular del planeta.
			</p><img src="Perro.png" class="fotoperros"><br><br>

			Estado de los comederos
		
		</div>
		<button class="Rojo"><a href="javascript:infoperros()">Info Perros</a></button>
		<script>
			function infoperros(){
				document.getElementById("inforojo").style.display="block";
			}
			function cerrarr(){
				document.getElementById("inforojo").style.display="none";
			}

		</script>


		<div class="ventanaamarilla" id="infoamarillo">
						
		<div id="cerraramarillo"><a href="javascript:cerraram()"><img src="cerrar.png"></a></div>
			INFORMACIÓN DE TLACUACHES

			<! - Informacion obtenida de https://www.ngenespanol.com/animales/tlacuache-asi-es-el-marsupial-que-enfrento-al-inframundo/ ->
			<p class="textotlacuaches">
				El nombre por el cual se conoce popularmente a este marsupial mexicano viene del náhuatl, “tlacuatzin” (el pequeño que come fuego). “Zorro del monte” o “zarigüeya” son otras formas de llamarlo. 
				Por lo general, cuando se habla del tlacuache se está haciendo referencia a Didelphis virginiana (en el sur) y Didelphis marsupialis (en el norte), sin embargo, en México, existen otras seis especies de la familia Didelphidae:
				<br><br>
				La constitución física del tlacuache es robusta. Su rostro es largo y cónico. Sus orejas carecen de pelo. La cola, en mismas condiciones, le sirve para colgarse de los árboles.
				El peso y tamaño es muy variable, ya que estos dependen de la especie. Un ejemplo de lo anterior es la Marmosa mexicana de 15 centímetros, en promedio, o el Didelphis marsupialis de 45 (1 a 3 kilogramos en etapa adulta), aproximadamente.
			</p><img src="Tlacuache.png" class="fototlacuaches"><br><br>

			Estado de los comederos
		
		</div>
		<button class="Amarillo"><a href="javascript:infotlacuaches()">Info Tlacuaches</a></button>
		<script>
			function infotlacuaches(){
				document.getElementById("infoamarillo").style.display="block";
			}
			function cerraram(){
				document.getElementById("infoamarillo").style.display="none";
			}

		</script>


		<h2 id="user" type="text">
		</h2>
		<h2 id="action" type="text">
.		</h2>
		<h2 id="edo" type="text">
		</h2>

	</div>

	<script type="module"> 
	// Import the functions you need from the SDKs you need
	  import { initializeApp } from "https://www.gstatic.com/firebasejs/9.6.3/firebase-app.js";
	  // TODO: Add SDKs for Firebase products that you want to use
	  // https://firebase.google.com/docs/web/setup#available-libraries

	  // Your web app's Firebase configuration
	  const firebaseConfig = {
		apiKey: "AIzaSyBfFnre7ykXRoYM2c2sU-ISsdLw6KLuAj4",
		authDomain: "fireb1-8f0f5.firebaseapp.com",
		databaseURL: "https://fireb1-8f0f5-default-rtdb.firebaseio.com",
		projectId: "fireb1-8f0f5",
		storageBucket: "fireb1-8f0f5.appspot.com",
		messagingSenderId: "803539275159",
		appId: "1:803539275159:web:218a7c60a176550a3108d2",
		measurementId: "G-5X2CY8CBJB"
	  };

	  // Initialize Firebase
	  const app = initializeApp(firebaseConfig);
	  
	  import {getDatabase,set,get,update,remove,ref,child}
	  from "https://www.gstatic.com/firebasejs/9.6.3/firebase-database.js"
	  
	  const db=getDatabase();
	  
	  var ingresaAccion=document.querySelector("#ingresaAccion");
	  var edo=document.querySelector("#edo");	  
	  var user=document.querySelector("#user");
	  var action=document.querySelector("#action");
	  var botonVerde=document.querySelector("#verde");
	  var botonAzul=document.querySelector("#azul");
	  var botonRojo=document.querySelector("#rojo");
	  var botonAmarillo=document.querySelector("#amarillo");
	  
	  
	  function EditarDatosG(){
		const dbref = ref(db);
		get(child(dbref, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4" ))
        .then((snapshot)=>{
            if(snapshot.exists()){
            	edo = snapshot.val().Estado;
            	if(edo === "Activo"){
            		update(ref(db, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4"),{
	                Control: "G_"+ingresaAccion.value,
	           
		        })
		        .then(()=>{
		         	alert("Informacion Actualizada");
		        })
		        .catch((error)=>{
		                alert(error);
		        });

            	} else{
            		alert("Usuario inactivo");
            	}
                    
            } else {
                    alert("No data found");
            }
        })
        .catch((error)=>{
            alert(error)
        })
	  }

	  function EditarDatosB(){

	  	const dbref = ref(db);
		get(child(dbref, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4" ))
        .then((snapshot)=>{
            if(snapshot.exists()){
            	edo = snapshot.val().Estado;
            	if(edo === "Activo"){
            		update(ref(db, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4"),{
	                Control: "B_"+ingresaAccion.value,
	           
		        })
		        .then(()=>{
		         	alert("Informacion Actualizada");
		        })
		        .catch((error)=>{
		                alert(error);
		        });

            	} else{
            		alert("Usuario inactivo");
            	}
                    
            } else {
                    alert("No data found");
            }
        })
        .catch((error)=>{
            alert(error)
        })

		
	  }
	  
	  function EditarDatosR(){
		const dbref = ref(db);
		get(child(dbref, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4" ))
        .then((snapshot)=>{
            if(snapshot.exists()){
            	edo = snapshot.val().Estado;
            	if(edo === "Activo"){
            		update(ref(db, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4"),{
	                Control: "R_"+ingresaAccion.value,
	           
		        })
		        .then(()=>{
		         	alert("Informacion Actualizada");
		        })
		        .catch((error)=>{
		                alert(error);
		        });

            	} else{
            		alert("Usuario inactivo");
            	}
                    
            } else {
                    alert("No data found");
            }
        })
        .catch((error)=>{
            alert(error)
        })
	  }
	  
	  function EditarDatosY(){
		const dbref = ref(db);
		get(child(dbref, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4" ))
        .then((snapshot)=>{
            if(snapshot.exists()){
            	edo = snapshot.val().Estado;
            	if(edo === "Activo"){
            		update(ref(db, "fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4"),{
	                Control: "Y_"+ingresaAccion.value,
	           
		        })
		        .then(()=>{
		         	alert("Informacion Actualizada");
		        })
		        .catch((error)=>{
		                alert(error);
		        });

            	} else{
            		alert("Usuario inactivo");
            	}
                    
            } else {
                    alert("No data found");
            }
        })
        .catch((error)=>{
            alert(error)
        })
	  }

	  const dbref = ref(db);
	  get(child(dbref,"fireb1-8f0f5-default/" + "-NgeTZgVRsPCfzDNOGD4"))
	  	.then((snapshot)=>{
	  		if (snapshot.exists()){
	  			edo.innerHTML = snapshot.val().Estado;
	  			document.getElementById("edo").innerHTML = edo.innerHTML;
	  			user.innerHTML = snapshot.val().Usuario;
	  			document.getElementById("user").innerHTML = user.innerHTML;
	  			action.innerHTML = "Ultima accion realizada: " + snapshot.val().Control
	  		}
	  	})

	  botonVerde.addEventListener("click",EditarDatosG);
	  botonAzul.addEventListener("click",EditarDatosB);
	  botonRojo.addEventListener("click",EditarDatosR);
	  botonAmarillo.addEventListener("click",EditarDatosY);	  
	</script>
	

</body></html>
