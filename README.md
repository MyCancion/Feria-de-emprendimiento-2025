# Feria-de-emprendimiento-2025
Sitio WEB de la feria

<!DOCTYPE html>

<html lang="es">
<head>
<meta charset="UTF-8">
<title>Feria de Emprendimiento 2025</title>

<style>
 
body {

background: linear-gradient(to right,#3b67f5, #059becac, rgb(113, 238, 247));
color: rgb(255, 255, 255);
display: flex;
flex-direction: column;
align-items:center;
justify-content: ri;
height: 100vh;
margin: 0;

}

h1 {
font-size: 3em;
margin-bottom: 30px;
text-shadow: 5px 5px 7px rgb(0, 0, 0);
font-family:'Orbitron', sans-serif;
}
 


.h1:hover {
transform: scale(1.05);

}


.contador {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 30px;
}

 .caja {
background-color:hsla(207, 89%, 44%, 0.034);
padding: 10px 10px;
border-radius: 15px;
box-shadow: 0 4px 10px rgb(239, 255, 16);
text-align: center;
transition: transform 0.3s;
 }

.numero {
font-size: 1.5em;
margin-bottom: 1px;

}

.texto {
font-size: 1em;
opacity: 0.8;
}

</style>
</head>
<body>
  
  <h1>Feria De Emprendimiento 2025</h1>

<div class="contador">
<div class="caja">
<div id="dias" class="numero">0</div>
<div class="texto">Días</div>
</div>
<div class="caja">
<div id="horas" class="numero">0</div>
<div class="text">Horas</div>
</div>
<div class="caja">
<div id="minutos" class="numero">0</div>
<div class="texto">Minutos</div>
</div>
<div class="caja">
<div id="segundos" class="numero">0</div>
<div class="texto">Segundos</div>
</div>
</div>

<script>
const fechaobjetivo =new Date(2025, 4, 15, 7, 0o0, 0o0); // 15 de Mayo de 2025

function actualizarCuentaRegresiva() {
const ahora = new Date().getTime();
const tiempoRestante = fechaobjetivo - ahora;
  
  if (tiempoRestante <= 0) {
document.querySelector(".contador").innerHTML = "<h2>¡ Tiempo terminado!</h2>";
clearInterval(intervalo);
return;

}

const dias = Math.floor(tiempoRestante / (1000 * 60 * 60 * 24));
const horas = Math.floor((tiempoRestante % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
const minutos = Math.floor((tiempoRestante % (1000 * 60 * 60)) / (1000 * 60));
const segundos = Math.floor((tiempoRestante % (1000 * 60)) / 1000);

document.getElementById("dias").textContent = dias;
document.getElementById("horas").textContent = horas;
document.getElementById("minutos").textContent = minutos;
document.getElementById("segundos").textContent = segundos;

}

const intervalo = setInterval(actualizarCuentaRegresiva, 1000);
actualizarCuentaRegresiva(); // Llamada inicial

</script>

</body>




 <div class="GASTRO">
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background-color: #111;
    }

    .GASTRO .boton-portada {
      display: block;
      position: relative;
      top: 90px;
      right: 330px;
      width: 100%;
      max-width: 150px;
      margin: 40px auto;
      text-decoration: none;
      color: inherit;
    }

    .GASTRO .boton-portada img {
      width: 100%;
      display: block;
      border-radius: 5px;
    }

    .GASTRO .titulo {
      position: absolute;
      top: 100px;
      left: 50%;
      transform: translateX(-50%);
      color: #ff0000;
      font-size: 1.5em;
      font-weight: bold;
      text-shadow: 2px 2px 8px black;
      font-family: 'Orbitron', sans-serif;
    }

    .GASTRO .boton-portada:hover {
      transform: scale(1.03);
      transition: transform 0.2s ease-in-out;
    }
  </style>
  
</head>


<body>
  
  <div class="GASTRO">
<a class="boton-portada" href="gastronomia.html" target="_blank">
  <img src="gastro.jpg" alt="Gastronomia">
  <div class="titulo">Gastronomia</div>
</a>
</body>




  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background-color: #111;
    }
  
    .HOTEL .boton-portada {
      display: flex;
      position: relative;
      top: -50px;
      right:120px;
      width:100%;
      max-width: 150px;
      margin: 40px auto;
      text-decoration: none;
      color: inherit;
    }
  
    .HOTEL .boton-portada img {
      width: 100%;
      display:flex;
      border-radius: 5px;
    }
  
    .HOTEL .titulo {
      position: absolute;
      top: 110px;
     left: 55px;
     transform: translateX(-30%);
      color: #ff0000;
      font-size: 1.5em;
      font-weight: bold;
      text-shadow: 2px 2px 8px rgb(0, 0, 0);
      font-family: 'Orbitron', sans-serif;
    }
  
    .HOTEL .boton-portada:hover {
      transform: scale(1.03);
      transition: transform 0.2s ease-in-out;
    }
  </style>
  </head>
  <body>
   
   
    <div class="HOTEL">
   <a class="boton-portada" href="hoteleria.html" target="_blank">
   <img src="hotel.jpg" alt="Hoteleria">
   <div class="titulo">Hoteleria </div>
   </a>
 </div>

 

  
 <style>
  body {
    margin: 0;
    font-family: sans-serif;
    background-color: #111;
  }

  .infor .boton-portada {
    display: flex;
    position: relative;
    top:-190px;
    right:-90px;
    width:100%;
    max-width: 150px;
    margin: 40px auto;
    text-decoration: none;
    color: inherit;
  }

  .infor .boton-portada img {
    width: 100%;
    display: block;
    border-radius: 5px;
  }

  .infor .titulo {
    position: absolute;
    top: 110px;
   left: 50px;
   transform: translateX(-30%);
    color: #ff0000;
    font-size: 1.5em;
    font-weight: bold;
    text-shadow: 2px 2px 8px black;
    font-family: 'Orbitron', sans-serif;
  }

  .infor .boton-portada:hover {
    transform: scale(1.03);
    transition: transform 0.2s ease-in-out;
  }
 </style>
 </head>
 <body>
 
  <div class="infor">
 <a class="boton-portada" href="informatica.html" target="_blank">
 <img src="infor.jpg" alt="Informatica">
 <div class="titulo">Informatica</div>
 </a>
 </div>

 <style>
  body {
    margin: 0;
    font-family: sans-serif;
    background-color: #111;
  }

  .agrope .boton-portada {
    display: flex;
    position: relative;
    top: -330px;
   left:300px;
    width:100%;
    max-width: 150px;
    margin: 40px auto;
    text-decoration: none;
    color: inherit;
  }

  .agrope .boton-portada img {
    width: 100%;
    display: block;
    border-radius: 5px;
  }

  .agrope .titulo {
    position: absolute;
    top: 115px;
   left: 45px;
   transform: translateX(-30%);
    color: #ff0000;
    font-size: 1.5em;
    font-weight: bold;
    text-shadow: 2px 2px 8px black;
    font-family: 'Orbitron', sans-serif;
  }

  .agrope .boton-portada:hover {
    transform: scale(1.03);
    transition: transform 0.2s ease-in-out;
  }
 </style>
 </head>
 <body>
 
  <div class="agrope">
 <a class="boton-portada" href="agropecuaria.html" target="_blank">
 <img src="agrope.jpg" alt="Agropecuaria">
 <div class="titulo">Agropecuaria</div>
 </a>
 </div>

</div>





</html>
