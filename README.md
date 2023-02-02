# weirdJS
Cosas raras que nos encontramos en javascript


```js
console.log( 0.1 + 0.2 === 0.3) // false
```

FALSE, resultado = 0.30000000000000004.

En JavaScript. Los números binarios de coma flotante 0.1 y 0.2 no son muy precisos. El resultado de su suma no es exactamente igual a 0.3, pero un número más cercano 0.30000000000000004, por lo que el resultado del juicio de condición esfalse。


```js
function print(first, second, first){ 
  console.log(first, second, first);
}
print(1, 2, 3); // 3 2 3 
```

El fragmento de código anterior tiene parámetros duplicados en el primer y tercer parámetro, el valor del primer parámetro se asigna al tercero que se pasa a la función, por lo tanto el tercer argumento anula el primer parámetro.
