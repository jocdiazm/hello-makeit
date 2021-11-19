# Ejercicio práctico

**Taller: Ejercicios Práctico**

1. Usar la etiqueta `<mark>` dentro de varios párrafos y explicar para qué sirve y cómo funciona.

2. **Displays**: Prepara tres divs con un tamaño de 100x100, cambia sus displays (block, inline, inline-block, none), observa y explica cómo se comportan.

3. **Imagen en párrafo**: Dentro de un párrafo de texto incluir una imagen de 100x100 y explicar cómo se distribuye el contenido.

4. **Imagen entre párrafos:** Entre dos párrafos añadir una imagen de 200x200 y explicar cómo se distribuye el contenido.

5. **Ajustando imágenes**: Hacer un div de 100x100px usando las propiedades width y height, incluir dentro una imagen de 100x100px y probar:

**a.** Añadir un `padding` de 10px.

**b.** Añadir un `borde` de 5px.

**c.** Cambiar el modelo de caja a `border-box` y explica qué ha pasado.

**d.** Centrar la caja utilizando el valor auto en los márgenes horizontales.

Los resultados o respuestas de sus análisis, entendimiento debe agregarlos aca.

## Solución

1. La etiqueta `<mark>`  funciona para resaltar texto dentro de Html. Ejemplo: 

```html
// Resalta las palabras "medellin, colombia"
José Carlos vive en <mark> medellín, colombia </mark>
```

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled.png)

1. **Displays de divs**

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%201.png)

- **Block:** Los elementos se organizan en forma de columna y tienen espacios entre ellos
- **Inline:** Los elementos se organizan en forma de filas y no toleran espacio arriba o abajo
- **inline-block:** Los objetos se organizan en filas y permiten tener espacios arriba y abajo
- **None:** los objetos "desaparen" nose muestran

1. **Como interactua una imágen con los párrafos:**

```html
<!DOCTYPE html>

<body>
    <p>
    Muy lejos, más allá de las montañas de palabras, alejados de los países de las vocales.
    Viven aislados en casas de letras, en la costa de la semántica, un gran océano de lenguas.
    <img src="https://falabella.scene7.com/is/image/FalabellaCO/3846190_6?wid=800&hei=800&qlt=70" width="100" height="100" alt="" srcset="">
    Un riachuelo llamado Pons fluye por su pueblo y los abastece con las normas necesarias.
    </p>    
</body>
</html>
```

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%202.png)

*La imagen queda contenida como si fuese una palabra más dentro del elemento de párrafo*

1. Al incluir la imágen queda separados los párrafos por la imagen, como se muestra a continuación:

```html
<p> Muy lejos, más allá de las montañas de palabras, alejados de los países de las vocales.
Viven aislados en casas de letras, en la costa de la semántica, un gran océano de lenguas. </p>

<img src="https://falabella.scene7.com/is/image/FalabellaCO/3846190_6?wid=800&hei=800&qlt=70" width="200" height="200" alt="" srcset="">
       
<p>Un riachuelo llamado Pons fluye por su pueblo y los abastece con las normas necesarias.</p>
```

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%203.png)

1. a. Añadiendo un padding de 10px el div se agranda y se mueve 10px en todas las direcciones desde un punto de fuga en la esquina superior izquierda

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%204.png)

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%205.png)

b. Añadiendo un borde de 5px muestra el padding de 10px inicial 

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%206.png)

c. Cambiando el border box, cosas malas le han pasado a la gente buena. La propiedad `box-sizing: border-box` dice al navegador tomar en cuenta para cualquier valor que se especifique de borde o de relleno para el ancho o alto de un elemento lo cual hace que la imagen "ya no quepa" porque se había definido la imágen con el mismo tamaño que el div (100x100 px) y el padding :

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%207.png)

d. Cambiando la propiedad `margin:auto;` del div, la caja se mueve al centro del canvas del navegador, de forma horizontal

![Untitled](Ejercicio%20pra%CC%81ctico%202b58c2a40588494399e485312ae8e4ef/Untitled%208.png)