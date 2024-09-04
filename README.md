
# 100 Preguntas sobre Javascript

[![](https://img.shields.io/badge/README-English-blue)](./README.en.md)

JavaScript es uno de los lenguajes de programación más populares del mundo, esencial para el desarrollo web y un conocimiento imprescindible para los desarrolladores de software. Ya sea que estés preparándote para una entrevista de trabajo o repasando tus conocimientos de JavaScript, esta lista completa de 100 preguntas y respuestas te ayudará a solidificar tu comprensión de JavaScript.

<details>
<summary>1- ¿Qué es JavaScript?</summary>

  **Respuesta**: JavaScript es un lenguaje de programación de alto nivel, dinámico, no tipado e interpretado. Se utiliza principalmente para crear contenido interactivo y dinámico en las páginas web. JavaScript es versátil y puede ser utilizado tanto en el lado del cliente como en el lado del servidor (Node.js).

JavaScript permite a los desarrolladores crear aplicaciones web enriquecidas mediante la manipulación del DOM (Modelo de Objeto de Documento), el manejo de eventos y la comunicación con servidores a través de solicitudes AJAX. También es una tecnología fundamental de la web, junto con HTML y CSS.

</details>

<details>
<summary>2. ¿Cuáles son los diferentes tipos de datos en JavaScript?</summary>

  **Respuesta**: 
  1. Tipos de Datos Primitivos:
     - String: Representa una secuencia de caracteres, por ejemplo, "¡Hola, Mundo!".
     - Number: Representa números enteros y de punto flotante, por ejemplo, 42 o 3.14.
     - Boolean: Representa entidades lógicas con dos valores: true o false.
     - Undefined: Una variable que ha sido declarada pero no se le ha asignado un valor tiene el tipo undefined.
     - Null: Representa la ausencia intencional de cualquier valor de objeto, a menudo se utiliza para indicar "sin valor".
     - Symbol (ES6): Un valor primitivo único e inmutable que se utiliza como clave de una propiedad de objeto.
     - BigInt (ES2020): Representa enteros con precisión arbitraria, lo que permite la manipulación de números enteros grandes más allá del límite de enteros seguros para los números.

  2. Tipos de Datos No Primitivos:
     - Object: Una colección de pares clave-valor, a menudo utilizada para almacenar datos y entidades más complejas.

> Entender estos tipos de datos es crucial para la manipulación de variables y la ejecución de funciones en JavaScript.
</details>

<details>
<summary>3. ¿Cuál es la diferencia entre `undefined` y `null` en JavaScript?</summary>

  **Respuesta**: En JavaScript, `undefined` y `null` son valores distintos que representan la ausencia de un valor, pero se utilizan en diferentes contextos:

`undefined`: Una variable es `undefined` cuando ha sido declarada pero aún no se le ha asignado un valor. Representa una falta de inicialización.

Ejemplo:
```javascript
let a;
console.log(a); // Salida: undefined
```

`null`: Una variable es `null` cuando se le asigna explícitamente un valor nulo. Representa la ausencia intencional de cualquier objeto o valor.

Ejemplo:
```javascript
let b = null;
console.log(b); // Salida: null
```

> Aunque ambos `undefined` y `null` se utilizan para denotar "sin valor", `undefined` es usualmente el estado por defecto de las variables no inicializadas, mientras que `null` es establecido explícitamente por el programador para indicar que una variable no debería tener valor.
</details>

<details>
<summary> 4. ¿Qué son los closures en JavaScript y por qué son útiles? </summary>

  **Respuesta**: Un closure es una característica en JavaScript donde una función interna tiene acceso a las variables de la función externa (que la envuelve), incluso después de que la función externa ha terminado de ejecutarse. Los closures se crean cada vez que se crea una función, en el momento de la creación de la función.

**Cómo funcionan los Closures**: Los closures permiten a las funciones "recordar" su ámbito léxico, permitiéndoles acceder a variables de su ámbito externo incluso cuando la función se ejecuta fuera de ese ámbito.

Ejemplo de un Closure:

```javascript
function outerFunction(outerVariable) {
  return function innerFunction(innerVariable) {
    console.log('Variable Externa: ' + outerVariable);
    console.log('Variable Interna: ' + innerVariable);
  };
}

const newFunction = outerFunction('fuera');
newFunction('dentro');
// Salida:
// Variable Externa: fuera
// Variable Interna: dentro
```

En este ejemplo, `innerFunction` conserva el acceso a `outerVariable` de `outerFunction` incluso después de que `outerFunction` ha terminado de ejecutarse.

Casos de Uso de los Closures:
- **Encapsulación de Datos**: Los closures se pueden usar para crear variables o métodos privados dentro de una función.
- **Callbacks**: Los closures se usan comúnmente con callbacks en programación asincrónica, como manejadores de eventos o setTimeouts.
- **Programación Funcional**: Los closures permiten patrones de programación funcional, permitiendo que las funciones se compongan y reutilicen.

> Los closures son herramientas poderosas en JavaScript que permiten ocultar datos y gestionar el estado, lo que los hace esenciales para construir aplicaciones complejas.

</details>

---

## Contribuyendo
Las contribuciones son lo que hace que la comunidad de código abierto sea un lugar increíble para aprender, inspirarse y crear. Agradecemos enormemente cualquier contribución que realices.

### Cómo Contribuir
* Haz un fork del proyecto
* Crea tu rama de característica (git checkout -b feature/AmazingFeature)
* Realiza tus cambios (git commit -m 'Agrega una característica increíble')
* Sube a la rama (git push origin feature/AmazingFeature)
* Abre un Pull Request

### Pautas para Contribuyentes

* Sigue el estilo de codificación y las pautas descritas en el archivo CONTRIBUTING.md.
* Asegúrate de que tu código pase todas las pruebas antes de enviarlo.
* Mantén tus commits organizados y claros.
* Siéntete libre de abrir un issue para cualquier solicitud de característica o reporte de error.

# Contribuyentes
¡Gracias a todas las personas increíbles que han contribuido a este proyecto!

<a href="https://github.com/holasoymalva/100-questions-about-javascript/graphs/contributors"> <img src="https://contrib.rocks/image?repo=holasoymalva/100-questions-about-javascript"/></a>

## Nuevos Contribuyentes
¡Damos la bienvenida a nuevos contribuyentes al proyecto! Si deseas ser parte de esta iniciativa, simplemente sigue los pasos en la sección Cómo Contribuir anterior. ¡Estamos encantados de revisar pull requests y colaborar para mejorar el proyecto juntos!

## Licencia

Distribuido bajo la Licencia MIT. Consulta el archivo LICENSE para obtener más información.
