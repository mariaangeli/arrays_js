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

## Accediendo a la información de un array

### Propiedad length
- Devuelve la cantidad de elementos del array

### Operador [pos]
-Permite acceder para leer o modificar el elemento pos del array

### Método at [pos]

-Devuelve el elemento de la posición pos. El parámetro admite valores negativos, lo que significa que empiezan a contar por el final del array.

```Javascript
const letters = ["A", "B", "c"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

### Añadir o eliminar elementos
-push(ele1, ele2): añade uno o varios elementos al final del array. Devuelve el tamaño del array.

```Javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agrega el elemento 4 al final del array
console.log(miArray);
```
- pop(): Devuelve el ultimo elemento del array y lo elimina

```Javascript
let miArray = [1, 2, 3];
miArray.pop(); // Elimina el ultimo elemento del array
console.log(miArray);
```
- unshift(ele1, ele2): Añade uno o varios elementos al inicio devolviendo el tamaño del array despues de añadidos

```Javascript
let miArray = [1, 2, 3];
miArray.unshi(0); // Agrega el elemento 0 al inicio del array
console.log(miArray);
```
-shift(): Devuelve el primer elemento del array y lo elimina

```Javascript
let miArray = [1, 2, 3];
miArray.shift(0); // Elimina el primer elemento del array
console.log(miArray);
```
- Concat(ele1, ele2): concatema de dos arrays

```Javascript
let miArray = [1, 2, 3];
let miOtroArray = [4, 5]; 
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray)

```
- split (separador): Apartir de una cadena, crear un array dividiendo dicha cadena en elementos delimitados por separador.

```Javascript
let miString ="Hola, ¿como estás";
let miArray = miString.split(" ");
console.log(miArray);
```
- join(separador): apartir de un array, crea una cadena separando cada elemento 

```Javascript
let miArray = ["Hola,","¿cómo", "estas?"];
let miString = miArray.join(" "); 
console.log(miString);
```
## Búsqueda de elementos de un array

- includes(elemento):devuelve true o false si el elemento existe o no dentro del array
- indexOf(elemento):devuelve la posición de la primera aparición del elemento. Si no existe,devuelve -1.
- lastIndexOf(elemento): devuelve la posición de la ultima aparicion del elemento. Si no existe,devuelve -1.

## Modificar el array o crear fragmentos
- slice(inicio, fin): devuelve un array con los elementos desde la posición inicio hasta la posición fin, ambos excluidos.

## Ordenar elementos de un array
- reverse(): invierte el orden de los elementos del array
- sort(): ordena el array alfabeticamente
- sort(criterio): ordena el array con el criterio determinado por la función criterio.

## Borrar elementos de un array
- Se peude borrar el contenido de un elemento de un array poniendo su valor a null o asignando una cadena vacía " ".
- Para eliminar completamente un elemento del array se utiliza el operador delete.

## Recorrido de un array
1. Recorrer con un bucle clásico, pasando por todos los elementos.
```Javascript
var dis = ["lunes", "martes", "miercoles", "jueves", "viernees", "sabado", "domingo"];
for(i=0;i<dias.leng;i++)
{
    console.log(dias[i])
}
```
2. Recorrer con un while, pasando por todos los elementos 
los elementos.

```Javascript
var dis = ["lunes", "martes", "miercoles", "jueves", "viernees", "sabado", "domingo"];
var i = 0
while(i<dias.length)
{
    console.log(dias[i]);
    i++;
}
```
3. Usando la sentencia for..in.

```Javascript
var dis = ["lunes", "martes", "miercoles", "jueves", "viernees", "sabado", "domingo"];
for(let index in dias)
{
    console.log(dias[i]);
}
```
## Arrays multidimensionales 

```Javascript
cons matix = [ 
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```
- Recorrer una matiz utilizando bucles anidados
```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernees", "sabado", "domingo"];
for(i=0;i<matriz.lenth; i++)
{
    for(let j=0;matríz[i].length; j++)
    {
        console.log(matriz[i][j]);
    }
}
```

# Ejercicios 

1. Dada una lista de números separados por coma,calcular la suma , el mayor,el menor y la media de todos.

2. Introducir dos cadenas con elementos separados por coma, y con un botón concatenar las dos cadenas y mostrarlas en pantalla.

3. Introducir uno a uno los elementos en un array a través de un boton. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los botones de debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.