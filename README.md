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