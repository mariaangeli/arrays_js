# Arrays

- Un array es una sona de almacenamiento continuo, donde se pueden introducir varios valores cada uno de ellos ubicado en la posición que ocupa en el array.
- Tambien son denominados arreglo o vectores,y cuando son de dos dimensiones son llamados matrices.
- Los arrays brindan la capacidad de almacenar una colección de elementos y acceder a ellos de manera individual.
- Cada elemento se identifica mediante su posición en el array,denominado **indice**,y estos indices son siempre secuenciales.
- En javascript son altamente flexibles en terminos de los diferentes tipos de datos que podemos almacenar en cada posición del array.

## Crear un array

1. Declarando un array con el elementos en linea

```Javascript
let miArray = [1, 2, 3];
console.log(miArray);
```

2. Declarando un array con la sintaxis **new array()**

```Javascript``
let miArry = new Array [1, 2, 3];
console.log(miArray);
```

3. Declarando un array con un tamaño especifico utilizando la sintaxis **new Array** y asignando valores después:

```Javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```
4. Declarando un array con elementos de diferentes tipos de datos

```Javascript
let miArray4 = [1, "dos", true, {nombre: "juan", edad: 38}];
console.log(miArray);
```