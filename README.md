# Simplicita
J.C.G.A

Pasos para descargas proyecto:
1)
copiar el siguiente comando en el cmd en la ruta que quieras.
>>git clone https://github.com/woolfii/Simplicita/

2)doble click sobre index.html

-->Tarea 1: Un pequeño buscador a partir de una API
  existente.
  
  Este Problema fue relativamente simple pues no hace mucho realice un ejercicio cuyo algoritmo era sumamente parecido a este ejercicio.
  Lo primero que hice fue crear el input y un botón, al botón le añadí el evento onClick mediante el cual consumo el api con una función fetch, dentro de la función 
  sustituyo el endpoint con el valor obtenido del input, dicho input esta validado para no realizar la petición vacía, igualmente si la validación del backend regresa 
  un error el error es "cachado" lo cual lanza una alerta y recarga la página para que el usuario pueda seguir intentando.
  Este ejercicio esta realizado con react unicamente, se transpilo a js con Babel y se empaqueto con webpack por lo que el codigo utilizado es unicamente el admin.bundle.js
  pero adjunto tambien el archivo casa.js para que quede una version legible por si requieren leer el codigo.
  
 -->Tarea 2: Un link interesante.
    
  El segundo problema es un problema que aparenta ser más fácil de lo que en realidad resulto ser, de antemano diré que no he podido dar con el resultado, sin embargo, 
  como el correo dice que de no dar con este resultado por lo menos describamos los acercamientos o los enfoques usados para tratar de dar con la solución, lo primero que 
  hice fue revisar que es lo que hacía diferente la página cuando se seguían los pasos planteados, lo único que encontré fue una variable almacenada en la sessionStorage, 
  una variable llamada "tabSessionId" con lo que parece un id random generado con uuid, desconocí el funcionamiento de sessionStorage así que lo primero que hice fue investigar
  el funcionamiento en diferentes fuentes, encontré su funcionamiento y sus métodos para interactuar con los datos, trate desde consola de obtenerlos y cambiarlos y lo logre así que
  traté de transportar dichas funcionas y aplicarlas desde un script, sin embargo, no pude obtenerlas por lo cual seguí buscando información y encontré que este tipo de almacenamiento
  aunque se hospeda en el cliente están relacionadas con el dominio directamente por lo cual no puede ser ni leído ni actualizado desde fuera, salvo que se piratee de alguna manera,
  manera que intenté encontrar, pero no hallé, el siguiente enfoque que pensé ya que no podía setear la sessionStorage desde fuera del dominio fue hacer los pasos indicados, pero sin 
  que el usuario se dé cuenta por lo cual se me ocurrió hacer uso de un iframe oculto y de ahí obligar a seguir los links necesarios con un una función SetTimeout, sin embargo, 
  al parecer la página bloquea este tipo de intentos ya que no tiene permitida la carga de la página en los iframe. 
  Hasta aquí ya no se me ocurre que hacer así que busque soluciones directas para lograr el objetivo sin embargo no encontré nada útil, si tuviera más tiempo lo que haría seria 
  buscar más información sobre las sessionStorage y como setearlas desde fuera, en este punto si no lo logro quizá preguntar con colegas que pudieran tener experiencia en el tema,
  o quizá replantearme el problema desde el principio y buscar otra solución.

