<!DOCTYPE html>
<!-- saved from url=(0169)file:///C:/Users/mane_/OneDrive/Escritorio/%C3%9Altimo%20Semestre/Internet%20de%20las%20cosas/Segundo%20Parcial/RFID_y_Bluetooth_con_registro_en_BD/Prueba.html?Estado=0# -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=windows-1252">
	<title>Prueba</title>

	<style>
		body{text-align:center;}
	</style>
</head>

<body>
	<div id="Ingresar">
		<h1>Ingresar Datos (0-OFF / 1-ON)</h1>
		<h4>Estado del LED</h4>
		<form action="file:///C:/Users/mane_/OneDrive/Escritorio/%C3%9Altimo%20Semestre/Internet%20de%20las%20cosas/Segundo%20Parcial/RFID_y_Bluetooth_con_registro_en_BD/Prueba.html?Estado=0#">
		<label for="ingresaAccion"> Estado </label>
		<select name="Estado" id="ingresaAccion">
		<option value="0"> Apagado</option>
		<option value="1"> Encendido</option>
		</select>
		<br><br>
		</form>

		<button style="background-color:lightgreen; border-color:green" id="verde">GREEN</button>
		<button style="background-color:lightblue; border-color:blue" id="azul">BLUE</button>
		<button style="background-color:lightred; border-color:red" id="rojo">RED</button>
		<button style="background-color:lightyellow; border-color:yellow" id="amarillo">YELLOW</button>
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
	  			edo.innerHTML = "Estado: " + snapshot.val().Estado;
	  			user.innerHTML = "Usuario: " + snapshot.val().Usuario;
	  			action.innerHTML = "Ultima accion realizada: " + snapshot.val().Control;
	  		}
	  	})
	  botonVerde.addEventListener("click",EditarDatosG);
	  botonAzul.addEventListener("click",EditarDatosB);
	  botonRojo.addEventListener("click",EditarDatosR);
	  botonAmarillo.addEventListener("click",EditarDatosY);

	</script>


</body></html>
