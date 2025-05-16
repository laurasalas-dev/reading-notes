# Preguntas de la Introducción a JavaScript

## ¿Cuáles son los diferentes tipos de datos que se pueden utilizar en JavaScript y cómo se diferencian entre sí?
Existen 2 tipos:
### Tipos primitivos
* String: Texto. Va entre comillas
* Number: Números (enteros o decimales)
* Boolean: Verdadero o falso.
* Undefined: Cuando una variable existe pero no tiene valor
* Null: Valor vacío o nulo a propósito
* BigInt: Para trabajar con números muy grandes
* Symbol (avanzado): Valor único, usado para identificar cosas
### Tipos de datos de referencia 
* Object: Colección de pares clave-valor
* Array: Lista de elementos
* Function: Bloque de código reutilizable
### Diferencias
Los datos primitivos son simples y se almacenan directamente. En cambio, los datos de referencia son estructuras complejas y se almacenan por referencia (como un "enlace" a su contenido).


## ¿Cómo se utilizan las estructuras condicionales if y else en JavaScript, y qué propósito cumplen dentro de un programa?
Las estructuras condicionales if y else en JavaScript se usan para tomar decisiones en un programa, es decir, ejecutar ciertas instrucciones solo si se cumple una condición.
Permiten que el programa reaccione de forma diferente según los datos o situaciones.


## ¿Cuáles son los diferentes tipos de operadores en JavaScript y cómo se utilizan los operadores aritméticos para realizar cálculos?
Existen 3 tipos: aritméticos, de comparación, lógicos.
### Aritméticos
1. `+` (suma)
2. `-` (resta)
3. `*` (multiplicación)
4. `/` (división)
5. `%` (resto)

``` 
// Usos de los operadores aritméticos
let x=10,y=5;
let suma = x + y;
let resta = x - y;
let multiplicacion = x * y;
let division = x / y;
let modulo = x % y;

console.log(suma,resta,multiplicacion,division,modulo);
```
### De comparación
1. `==` (igualdad débil)
2. `===` (igualdad fuerte)
3. `!=` (desigualdad)
4. `>` (mayor)
5. `<` (menor)
6. `>=` (mayor igual)
7. `<=` (menor igual)
```
let debil = 5 == "5";
let fuerte = 5 === "5";
let desigualdad = 5 != "5";
let mayor = 10 > 5;
let menor = 10 < 5;
let maIgual = 5 >= 5;
let meIgual = 4 <= 5;

console.log(debil, fuerte, desigualdad, mayor, menor, maIgual, meIgual);
```

### Lógicos
1. `&&` (Y (AND))
2. `||` (O (or))
3.  `!` (negación)
```
let num1 = 3, num2=6;

let and = num1 && num2;
let or = num1 || num2;
let negacion = !num1;

console.log(and, or, negacion);
```

# ¿Cómo se declara una variable en JavaScript y cuáles son las diferencias entre var, let y const en cuanto a su alcance y mutabilidad?
Para declarar variables, se emplean 3 palabras clave: var, let, const.
Tienen diferencias importantes en cuanto a su alcance (dónde se puede usar la variable) y su mutabilidad (si se puede cambiar el valor o no).
* var: 
1- Solo vive dentro de la función donde fue declarada, no respeta los bloques como if o for.
2- Su valor puede cambiar.

* let:
1- Solo vive dentro del bloque { } donde se declara.
2- Sí se puede cambiar su valor después de declararla.
3- Se usa cuando necesitas una variable que pueda cambiar su valor, por ejemplo en bucles o condiciones.

* const:
1- No se puede re-declarar ni cambiar su valor después de asignarlo.
2- Si el valor es un objeto o un arreglo, puedes modificar su contenido interno, pero no puedes asignarle un nuevo objeto o arreglo.
3- Se usa cuando quieres asegurarte de que la variable no cambie, como una constante matemática o una configuración fija.