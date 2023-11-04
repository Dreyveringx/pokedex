Solución del Reto 19


¡Bienvenidos al reto 19! En este proyecto, se pidió recrear una interfaz que muestre tarjetas de Pokémon, donde cada tarjeta debe mostrar información relevante sobre un Pokémon específico, como su nombre, número de identificación, tipo y una imagen. Además, se proporcionó un video de explicación y recursos iniciales que incluyen una estructura HTML y parte del CSS, así como una pista sobre cómo obtener datos de la API pokeapi.co para completar el desafío. 

Aquí se detalla la solución implementada:

Implementación

Recursos Iniciales:

*Se proporciona una estructura HTML para el proyecto, que incluye un contenedor con el id 'poke-container' donde se deben agregar las tarjetas de Pokémon.
*También se proporcionó una estructura CSS parcial que define colores para diferentes tipos de Pokémon, lo que será útil para establecer el fondo de las tarjetas.

JavaScript (JS):

Se utilizó JavaScript para interactuar con la API pokeapi.co y obtener datos de Pokémon.


*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/
*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/
Crear Tarjetas de Pokémon:


*La función createPokemonCard crea una tarjeta para un Pokémon dado utilizando el DOM.

-Se crea un elemento div con la clase 'pokemon' y se le asigna un fondo de color basado en el tipo del Pokémon, utilizando los colores definidos en el objeto colors.
-Se crea un contenedor de imagen con la clase 'img-container' y se agrega una imagen del Pokémon.
-Se muestra el número de identificación del Pokémon y el nombre en la tarjeta.
-También se muestra el tipo del Pokémon en la tarjeta.

****Creación del Elemento de Tarjeta***

-Se crea un nuevo elemento div llamado card que servirá como la tarjeta de Pokémon.
-Se le asigna una clase pokemon utilizando classList.add('pokemon').
-Además, se establece el fondo de la tarjeta en función del tipo de Pokémon utilizando el color correspondiente del objeto colors. Esto se hace mediante la propiedad style.backgroundColor.

***Creación del Contenedor de Imagen***

-Se crea otro elemento div llamado imgContainer que servirá como el contenedor de la imagen del Pokémon.
-Se le asigna una clase img-container utilizando classList.add('img-container').

***Imagen del Pokémon***

-Se crea un elemento img llamado img que será la imagen del Pokémon.
-Se establece la fuente de la imagen (src) utilizando pokemon.sprites.front_default, que se obtiene de los datos del Pokémon proporcionados por la API.
-Se establece el atributo alt de la imagen en el nombre del Pokémon (pokemon.name), lo que facilita la accesibilidad.

***Número de Identificación del Pokémon***

-Se crea un elemento span llamado number que mostrará el número de identificación del Pokémon.
-Se le asigna una clase number utilizando classList.add('number').
-El número de identificación se formatea utilizando #${pokemon.id.toString().padStart(3, 0)}, lo que garantiza que el número siempre tenga tres dígitos rellenados con ceros a la izquierda si es necesario.

***Nombre del Pokémon***

-Se crea un elemento h3 llamado name que mostrará el nombre del Pokémon.
-Se le asigna una clase name utilizando classList.add('name').
-El nombre del Pokémon se capitaliza para que la primera letra esté en mayúscula, independientemente de cómo se encuentre en los datos de la API.

***Tipo del Pokémon***

-Se crea un elemento small llamado type que mostrará el tipo del Pokémon.
-Se asigna el tipo del Pokémon utilizando pokemon.types[0].type.name. Aquí, se asume que el Pokémon tiene un solo tipo (el primer tipo en la lista), por lo que se toma ese tipo.
-El tipo se muestra dentro de un elemento span para resaltar el tipo.


***Anidación de Elementos***

-Los elementos imgContainer, number, name, y type se anidan dentro del elemento card para crear la estructura de la tarjeta.

***Agregando la Tarjeta al Contenedor de Pokémon***

-Finalmente, la tarjeta (card) se agrega al contenedor principal de Pokémon (poke_container) en el documento HTML, lo que la hace visible en la página.


*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/
*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/*/

Instrucciones para Ejecutar el Proyecto

-Clonar o descargar el repositorio desde el [repositorio original](URL del repositorio original).

-Abra el archivo HTML en un navegador web para ver las tarjetas de Pokémon en acción.

-Asegúrese de tener una conexión a Internet para cargar los datos de la API pokeapi.co.

-Si desea personalizar el proyecto, puede modificar el HTML y el CSS según sus necesidades.

¡Eso es todo! Ahora tiene una solución funcional para el proyecto del Reto 19 que muestra tarjetas de Pokémon con datos obtenidos de la API pokeapi.co. ¡Diviértase explorando y personalizando este proyecto!