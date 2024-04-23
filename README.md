# arrays_js

# Arrays
 
- Una array es una zona de almacenamiento continuo donde se puede introducir varios valores, cda uno de ello ubicado por la posicion que ocupa en la array.
- tambien son denominados arreglos o vectores, y cuando son de dos dimenciones son llamados matrices.
- los array nos brinda capacidad de almacenar una cantidad de elementos y acceder a ellos de manera individual.
- cada elemento se identifica en su posicion en la array, denominada **indice**, y estos indices son siempre secuenciaoles.
- en js son altamente flexible en terminos de los diferentes tipos de datos que podemos almacenar en cada posicion del array.

## crear una array

1. Declarando una array con elemntos en en linea
```Javascript
let miArray = [1,2,3];
console.log(miArray);
```
2. declarando una array con la sintaxis **new Array()**
```Javascript
let miArray = new Array(1,2,3);
console.log(miArray);
```
3. declarando una array con un tamaño especifico utilizando la sintaxis de la array  **new Array** y asignando valores despues.
```Javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```
4. declarando una array con diferentes tipos de datos.
```Javascript
let miArray4 = [1,"dos", true, {nombre: "juan", edad: 30}]
console.log(miArray4);
```

## Accediendo a la informacion de una array

### Propiedad length
- Devuelve la cantidad de elelmentos de la Array.

### operador [pos]
- permite acceder para leer o modificar el elemento pos de la array.

### metodo at(pos)
- devulve el elemento de la posicion pos. el parametro permite valores negativos , lo que significa que empieza a contar por el final de la array.
```Javascript
const letters = ["A", "B", "C"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos 
- push(elel1, elel2): añade uno o mas elementos al final del Array. devuelve el tamaño de la array.
```Javascript
let miArray = [1,2,3];
miArray.push (4);// agrega el elemento 4 alfinal de la array
console.log(miArray);
```

-pop(): Devuelve el ultimo elemento de la array y lo elimina.
```Javascript
let miArray = [1,2,3];
miArray.pop();// elimina el ultimo elemento de la array
console.log(miArray);
```

- unshift(elel1, elel2): añade uno o varios elementos al inicio, devolviendo el tamaño del array despues del añadido
```Javascript
let miArray = [1,2,3];
miArray.unshift(0);// agrega el elemento 0 al inicio de la array
console.log(miArray);
```

- shift(): devuelve el primer elemento del array y lo elimina
```Javascript
let miArray = [1,2,3];
miArray.shift(0);// elimina el primer elemento de la array
console.log(miArray);
```

- concat(elel1, elel2): concatena dos Array
```Javascript
let miArray = [1,2,3];
let miOtroArray = [4,5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray);
```

- split(separador): a partir de una cadena, crea un array devidiendo dicha cadena en elementos delimitados por separador.
```Javascript
let miString ="hola, ¿como estas?";
let miArray = miString.split(" ");
console.log(miArray);
```

join(separador): a partir de un array. crea una cadena separada cada elemento con el separador.
```Javascript
let miArray = ["hola,", "¿como" , "estas?"];
let miString = miArray.join(" ");
console.log(miString);
```

## Busqueda de elementos en una array
- includes(elemento): devuelve true o false si el elemento existe o no dentro de la Array
- indexOf(elemento): devuelve la posicion de la primera aparicion del elemento. si no existe, devuelve -1.
- lasIndexOf(elemento): devuelve la posicion de la ultima aparicion del elemento. si no existe, devuelve -1.

## modificar el Array o crear fragmentos 
- slice(inicio, fin): devuelve un array con los elementos desde la posicion inicio hasta la posicion fin, ambos excluidos.

## ordenar elementos de una array
- reverse(): invierte el orden de los elementos del Array
- sort(): ordenar el array con el determinado por la funcion criterio.
- sort(criterio): ordena el array con el criterio determinado por la funcion criterio.

## Borrar elementos de un array

- Se puede borrar el contenido de un elemento de un array poniendo su valor a null o asignando una cadena vacia " ".

- Para elminar completamente un elemento del array se utiliza el operador delete.

## Recorrido de un array

1. Recorrer con un bucle clásico, pasando por todos los elementos.

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for (i=0; i<dias.length;i++)
{
    console.log(dias[i]);
}
```

2. Recorrer con while, pasando por todos los elementos

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
var i =0;
while(i=0; i<dias.length)
{
    console.log(dias[i]);
}
```

3. Usando la sentencia for..in.

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(let index in dias)
{
    console.log(dias[index]);
}
```

## Arrays multidimensionales 

```Javascript
const matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```

- Recorrer una matriz utilizando bucles anidados 

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for (let i=0; i<matriz.length;i++)
{
    for(let j=0;matriz[i]. length; j++)
    {
        console.log(dias[i][j]);
    }
}
```


# ejercicios

1. Dada una lista de números separados por coma, calcular la suma, el mayor, el menor y la media de todos.

2. Introducir dos cadenas con elementos seperados por coma, y con un botón concatenar las dos cadenas y mostrarlas en pantalla.

3. Introducir uno a uno los elementos en un array a través de un boton. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los botones de debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.