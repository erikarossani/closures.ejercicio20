
# closures.ejercicio20

##Contexto
###Ejercicio Inicial

```javascript

var num2 = 0;

function suma(num1) {
return function() {
return num1 + num2;
}
} 

var suma2 = suma(2);
console.log(suma2(5)); // Debería mostrar 7 de resultado

var suma12 = suma(12);
console.log(suma12(76)) // Debería mostrar 88 de resultado.
```
```javascript

###Resultado final del ejercicio final 
function suma(num1) {
return function() {
return num1 + num2;
}
} 

var suma2 = suma(2);
console.log(suma2(5)); 

var suma12 = suma(12);
console.log(suma12(76));
```

#### Explicación del ejercicio:
En el ejercicio inicial no se ejecuta porque la función anonima(función hijo) no recibe ningún argumento y por eso no se puede retornar a la suma (num1 + num2); por eso en el codigo final la función suma recibe un argumento num1 y retorna una función anonima. La función anonima que retorna recibe un argumento num2 y retorna la suma de num1 y num2. Eso convierte a suma() en una función capaz de crear otras funciones. En el codigo se usa suma() para crear dos funciones, la primera para sumar la variable (suma2 =  suma(2) num1 con el valor num2(5) y seria igual para la variable suma12. Y se elimino la variable global ya que se esta declarando dentro la función por eso no se necesita en este codigo.
