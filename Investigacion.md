El DOM (Document Object Model) es una representación en memoria de la estructura de un documento HTML (o XML) que proporciona una interfaz para acceder y manipular los elementos y contenido del documento. Esencialmente, el DOM organiza la estructura del documento en un árbol de nodos, donde cada nodo representa un elemento, atributo o texto en el documento.

Para modificar el DOM, puedes utilizar varias funciones y métodos proporcionados por JavaScript (u otros lenguajes que trabajen en conjunto con el DOM).

El DOM representa el documento como un árbol de objetos, donde cada elemento del documento (como encabezados, párrafos, enlaces, imágenes, etc.) se representa como un nodo en el árbol. Estos nodos pueden tener padres, hijos y hermanos, lo que refleja la estructura jerárquica del documento. Además, cada nodo puede tener propiedades y métodos que permiten a los desarrolladores interactuar con él de diversas formas, como cambiar su contenido, estilo o posición en la página.


El DOM es fundamental para la programación web, ya que permite a los desarrolladores crear páginas web interactivas y dinámicas mediante la manipulación de elementos HTML y la respuesta a eventos del usuario. JavaScript es uno de los lenguajes de programación más comunes que se utiliza para interactuar con el DOM en el lado del cliente de una aplicación web. Con JavaScript y el DOM, los desarrolladores pueden crear aplicaciones web interactivas y ricas en contenido.

  

¿Cuáles son las funciones que permite modificar el DOM?

  

1.- **Acceder a elementos:**

  

Para acceder a elementos en el DOM, se utilizan métodos como `getElementById` o `querySelector` para seleccionar elementos por su identificador único (ID) o por un selector CSS, respectivamente.

  ![[1.png]]
  

2.- **Acceder a elementos padre/hijo:**

  

Puedes acceder a elementos padres e hijos de un elemento específico utilizando las propiedades `parentNode`, `childNodes`, `children`, `firstChild`, `lastChild`, entre otras.

![[Pasted image 20230925115626.png]]

3.- **Crear elementos:**

  

Puedes crear nuevos elementos HTML utilizando el método `createElement`, y luego configurar sus propiedades y contenido antes de agregarlos al DOM.

  ![[Pasted image 20230925115654.png]]
4.- **Añadir elementos al DOM:**

  

Una vez que hayas creado un nuevo elemento, puedes agregarlo al DOM utilizando métodos como `appendChild`, `insertBefore` u otros métodos relacionados con la manipulación de nodos.

  
![[Pasted image 20230925115723.png]]
  

5.- **Añadir / Eliminar clases:**

  

Puedes agregar o eliminar clases CSS en elementos HTML para cambiar su estilo y presentación.

  ![[Pasted image 20230925115757.png]]

![[Pasted image 20230925115817.png]]
  

6.- **Obtener atributos:**

  

Puedes obtener el valor de los atributos de un elemento utilizando el método `getAttribute`.
![[Pasted image 20230925115841.png]]

7.- **Escribir texto dentro de un elemento:**

  

Puedes modificar el contenido de texto de un elemento utilizando la propiedad `textContent` o `innerHTML`.

  
![[Pasted image 20230925115904.png]]
8.- **Modificar atributos:**

  

Puedes modificar los atributos de un elemento directamente accediendo a sus propiedades.

  
![[Pasted image 20230925120104.png]]


jQuery es una biblioteca de JavaScript, que es un lenguaje de programación utilizado para crear páginas web interactivas y dinámicas. Piensa en jQuery como un conjunto de herramientas y funciones predefinidas que facilitan a los programadores trabajar con JavaScript y manipular elementos en una página web.

JavaScript es poderoso pero, a veces, escribir código puro en JavaScript para realizar tareas comunes puede ser un poco largo y complicado. Es ahí donde entra jQuery. Imagina que es como un paquete de herramientas que te ayuda a hacer cosas geniales con menos esfuerzo.

Por ejemplo, supongamos que quieres hacer que un botón cambie de color cuando alguien hace clic en él. Con JavaScript, tendrías que escribir varias líneas de código para lograrlo. Pero con jQuery, puedes hacerlo con solo unas pocas líneas de código. Simplifica y acelera la escritura de código.

Además, jQuery también aborda la compatibilidad entre navegadores. Antes, había diferencias en cómo funcionaba JavaScript en distintos navegadores, lo que podía causar problemas. jQuery se encarga de eso y asegura que tu código funcione de manera similar en todos los navegadores, evitando quebraderos de cabeza.

En resumen, jQuery es una herramienta que facilita la vida de los desarrolladores web. Permite hacer cosas increíbles en una página web de forma más rápida y sencilla, garantizando una experiencia web fluida y consistente en todos los navegadores.
Para invocar funciones en jQuery que te permitan acceder, crear, añadir, obtener atributos y escribir texto dentro de un elemento, así como modificar atributos, puedes usar las siguientes funciones y métodos proporcionados por jQuery:

1. **Acceder a un elemento (selección de elementos)**:
   Para acceder a un elemento en jQuery, utilizas selectores. Aquí tienes algunos ejemplos:

   ```javascript
   // Acceder a un elemento por su ID
   var elementoPorId = $('#miElemento');

   // Acceder a un elemento por su clase
   var elementosPorClase = $('.miClase');

   // Acceder a un elemento por su tipo
   var elementosPorTipo = $('p');
   ```

2. **Crear un elemento**:
   Para crear un elemento en jQuery, puedes usar la función `jQuery` o su alias `$` junto con el método `append` o `prepend`. Aquí tienes un ejemplo de creación de un elemento div:

   ```javascript
   var nuevoElemento = $('<div></div>');
   ```

3. **Añadir un elemento a otro (añadir elementos hijos)**:
   Puedes usar el método `append` para añadir un elemento como hijo de otro elemento.

   ```javascript
   $('#contenedor').append(nuevoElemento);
   ```

4. **Obtener o establecer atributos**:
   Para obtener o establecer atributos de un elemento en jQuery, puedes usar los métodos `attr` y `removeAttr`.

   ```javascript
   // Obtener el valor de un atributo
   var valorAtributo = $('#miElemento').attr('id');

   // Establecer un atributo
   $('#miElemento').attr('nuevoAtributo', 'valorNuevo');

   // Eliminar un atributo
   $('#miElemento').removeAttr('nuevoAtributo');
   ```

5. **Escribir texto dentro de un elemento**:
   Para escribir texto dentro de un elemento en jQuery, puedes usar el método `text`.

   ```javascript
   $('#miElemento').text('Este es el nuevo texto');
   ```

6. **Modificar atributos (como cambiar clases)**:
   Para modificar atributos como las clases de un elemento, puedes usar el método `addClass`, `removeClass` y `toggleClass`.

   ```javascript
   $('#miElemento').addClass('nuevaClase');
   $('#miElemento').removeClass('claseExistente');
   $('#miElemento').toggleClass('toggleClase');
   ```

