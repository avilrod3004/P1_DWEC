# 5. Modelo de ejecución
Las aplicaciones web se desarrollan siguiendo una arquitectura cliente-servidor:
- **Cliente:** es el navegador web del usuario, que hace peticiones al servidor para obtener datos, enviar información o interactuar con la aplicación. El código que se ejecuta el navegador abarca los lenguajes HTML, CSS y JavaScript. Ejemplos de uso: validaciones de formularios y manejo de eventos en la página. 
- **Servidor:** recibe las peticiones del cliente a través de la red. Se encarga de responder las peticiones del cliente, almacenar la información, el procesamiento de datos y el control de las reglas de negocios. El código que ejecuta suele ser PHP, Python, Java, Node.js, etc. Ejemplos de uso: autenticación de usuarios y procesamiento de transacciones.


# 6. Lenguajes de programación web
Los lenguajes usados en el lado del cliente son:
- **JavaScript:** fue creado en 1995 para hacer las páginas web interactivas y dinámicas. Una de sus características es su tipado dinámico, no hay que especificar el tipo de dato al declarar una variable.
- **TypeScript:** fue creado en 2012 por Microsoft. Está basado en JavaScript, pero con características, herramientas y funciones adicionales que hacen que sea más ágil y seguro. Al contrario que JavaScript, TypeScript es de tipado estático. Esto hace que el código sea más robusto y sencillo de mantener.

Diferencias:
| JavaScript | TypeScript |
| -- | -- |
| Lenguaje interpretado | Compilado a JavaScript |
| Tipado dinámico | Tipado estático |
| Usado para proyectos pequeños o medianos | Usado para proyectos grandes y complejos |
| Soporta POO pero de manera menos tradicional | Soporte más robusto para POO |

# 7. Tecnologías seleccionadas

## 7.1. Evaluación de los mecanismos de integración de lenguajes de marcas con lenguajes de programación de clientes web
Como lenguaje de programación he elegido JavaScript para desarrollar la parte del cliente y del servidor, con Node.js.
Gracias a la manipulación del DOM con JavaScript podré convertir la estructura base de la página web hecha en HTML y CSS en una aplicación interactiva.

## 7.2. Evaluación de herramientas de programación para clientes web
Las herramientas que he seleccionado son:
- **WebStorm:** Es un IDE desarrollado por JetBrains. Elijo este porque incluye desde el principio complementos que en otros editores de código hay que instalar manualmente.
- **Frameworks:** React porque permite crear de manera eficiente interfaces de usuario interactivas y atractivas. Express porque es de los frameworks más populares para Node.js, es minimalista y eficiente en el manejo de peticiones HTTP.
- **Babel:** Es un transpilador para evitar problemas de compatibilidad entre los navegadores, de esta manera podrá ejecutarse incluso en navegadores con versiones antiguas.

# 8. Compatibilidad en navegadores
> ECMAScript es el estándar creado para homogenerizar como JavaScript es implementado en cada navegador.

Las versiones ES1 a ES5 son compatibles con todos los navegadores. ECMAScript 2015 está disponible en todos los navegadores actuales (Internet Explorer y clientes que ya no se actualizan no lo pueden interpretar). Las versiones posteriores de ECMAScript cada navegador las incorpora a su ritmo, es decir no siempre las novedades del último año están disponibles en todos los navegadores. Chrome suele ser el más rápido en adoptarlas.

Para conocer el estado de un navegador respecto a una especificación de ECMAScript se puede consultar la tabla de compatibilidad de Kangax (https://compat-table.github.io/compat-table/es6/).

Para evitar problemas de compatibilidad se usan transpiladores como Babel. Pasan el código nuevo a código seguro para que pueda funcionar en cualquier dispositivo. Por ejemplo, las funciones flecha las convierte en funciones normales en navegadores que no son compatibles con ECMAScript6.

También pueden surgir problemas de compatibilidad con los lenguajes de marcas HTML y CSS para hacerles frente se usan poyfills para emular las funcionalidades no soportadas.
