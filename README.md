# weirdJS
Cosas raras que nos encontramos en javascript

<hr>

```js
console.log( 0.1 + 0.2 === 0.3) // false
```

FALSE, resultado = 0.30000000000000004.

En JavaScript. Los números binarios de coma flotante 0.1 y 0.2 no son muy precisos. El resultado de su suma no es exactamente igual a 0.3, pero un número más cercano 0.30000000000000004, por lo que el resultado del juicio de condición esfalse。

<hr>

```js
function print(first, second, first){ 
  console.log(first, second, first);
}
print(1, 2, 3); // 3 2 3 
```

El fragmento de código anterior tiene parámetros duplicados en el primer y tercer parámetro, el valor del primer parámetro se asigna al tercero que se pasa a la función, por lo tanto el tercer argumento anula el primer parámetro.

<hr>

```js
[] == ![]; // -> true
+[] == +![]; // -> true
```

El comparador de igualdad convierte ambos miembros a número para compararlos, y ambos miembros pasan a ser 0 por diferentes motivos.

```js
[] == ![]; // -> 0 == 0 -> true
```

<hr>


```js
var y = 1;
if (function f() {}) {
    y += typeof f;
}
console.log(y);
```

El if lo toma con un literal lo cual entra en la condición. El resultado va a depender del motor, para el caso de Chrome el resultado es la concatenación de 1undefined, para el caso de EDGE, 1object. 

<hr>
