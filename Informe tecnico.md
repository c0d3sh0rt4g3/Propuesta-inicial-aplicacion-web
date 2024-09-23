# Informe técnico

### Índice

1. [Análisis modelos de ejecución cliente/servidor](#análisis-modelos-de-ejecución-clienteservidor)
2. [Evaluación lenguajes de programación web utilizados](#evaluación-lenguajes-de-programación-web-utilizados)
3. [Problemas de compatibilidad entre navegadores](#problemas-de-compatibilidad-entre-navegadores)

### Análisis modelos de ejecución cliente/servidor

El modelo cliente/servidor consiste en dos entidades: el cliente y el servidor. Siendo el cliente el que realiza 
solicitudes, mientras que el servidor se encarga de responder a estas solicitudes y proporcionar recursos o servicios,
existen 3 arquitectuiras comunes dentro del modelo cliente/servidor:

 **Modelo cliente/servidor de 2 capas (2 tier)** <br>
 Es el modelo habitual, el cliente se comunica directamente con el servidor, la logica de la aplicación de divide en 2 partes 
 la interfaz de usuario en el lado del lciente y los datos que se procesan, en el servidor, un ejemplo de una aplicación 
 que siga esta arquitectura sería una aplicación paea gestionar las existencias del almacén de una tienda pequeña.
 
**Modelo cliente/servidor de 3 capas (3 Tier)** <br>
En este modelo, la lógica de nuestra app se divide en 3 capas: Interfaz de usuario, lógica de negocio y base de datos, 
es decir, que el cliente se conecta a un servidor que, a su vez, interactua con una base de datos, un ejemplo de una 
aplicación de este tipo sería una aplicación de un e-commerce donde, en el lado del cliente, muestra los productos y 
permite añadirlos al carrito para realizar pedidos, en la lógica de negocio tiene una API para gestionar los productos, 
usuarios y pedidos, así como gestionar pagos cconectandose a una API externa y por último, en el lado del a base de datos,
almacena los datos de los usuarios, los productos, las transacciones y los pedidos realizados

**Tabla comparativa resumen de los 2 modelos:**

|               | 2 capas (2 tier)                      | 3 capas (3 tier)               |
|---------------|---------------------------------------|--------------------------------|
| Dificultad    | Baja                                  | Media                          |
| Escalabilidad | Limitada                              | Moderada                       |
| Mantenimiento | Dificil debido a la logica acoplada   | Centralizado en el servidor    |
| Latencia      | Baja debido a la comunicacion directa | Moderada                       |
| Uso           | Aplicaciones pequeñas/locales         | Aplicaciones Web empresariales |

### Evaluación lenguajes de programación web utilizados
He decidido utilizar **Javascript con React** para mi propuesta debido a su caracter modular, ya que al usar componentes,
reutilizar estos en la aplicación haría el trabajo más comodo y eficiente además, al utilizar un DOM virtual mejora el
rendimiento de la aplicación, no todo es positivo a la hora de utilizar **Javasript con React**, ya que a medida que crezca 
mi aplicación, se me puede llegar a complicar la gestión de los estados además, ya que react está en constante desarrollo, 
esto me obligará a mantener la aplicación al día con las nuevas herramientas que se desarrollen en versiones más nuevas

### Problemas de compatibilidad entre navegadores
Los problemas de compatibilidad que me puedo llegar a encontrar entre navegadores son los siguientes:
<br>
**Validación de HTML y CSS**<br>
Puesto que cada navegador lee y gestiona de forma diferente el codigo que lee, por ejemplo, los pequeños errores que un
navegador puede que solucione automaticamente, llevandonos a que, en el navegador donde no se solvente solo este error, 
no se muestre la página tal y como se busca, para evitar este problema, la mejor decision que podemos tomar es utilizar 
validadores de CSS como **Jigsaw CSS Validator**.<br>
**Falta de resets CSS**<br>
Cada navegador tiene sus propios presets de CSS y por tanto puede que algunos elementos que no se hayan modificado puesto
que no suponian un problema en el navegador donde se desarrolló, en otro navegador se muestren distintos, la solución
para este problema es usar una hoja de reset de estilos, sobreescribiendo asi los valores default de cada navegador.<br>
**Problemas con JavaScript**<br>
Al utilizar funciones mordernas de Javascriot, es posible que en no todos los navegadores funcionen, debido a que la 
version de ECMAScript que utiliza cada navegador no tiene por qué ser la misma en todos, para evitar estos problemas,
lo que podemos hacer es, antes de usar un método novedoso, buscarlo en [Can I use...](https://caniuse.com/) para consultar
la compatibilidad de este.<br>
### Bibliografía
[Todo sobre la arquitectura cliente-servidor](https://www.arsys.es/blog/todo-sobre-la-arquitectura-cliente-servidor)<br>
[Arquitectura Cliente/Servidor: modelo de 3 capas](https://iberasync.es/arquitectura-cliente-servidor-modelo-de-3-capas/)<br>
[Advantages and Disadvantages of React JS](https://medium.com/@reactmasters.in/advantages-and-disadvantages-of-react-js-e6c80b25763b)<br>
[Formas de evitar los problemas de compatibilidad multi navegador](https://comparium.app/es/blog/cross-browser-compatibility-issues/)