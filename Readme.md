*MÓDULO SOBRE REACT JS*

# Preguntas teóricas

1. Explicar brevemente el concepto de ReactJS y sus principales características.
R//: 
React es una librería de JavaScript para construir interfacez de usuario reactivas e interactivas. Sus principales características son las siguientes:
- Usa el virtual DOM para tener un mejor desempeño y rendimiento al minizar los cambios directos en el DOM.
- Organiza la interfaz en componentes reutilizables.
- Permite escribir código HTML dentro de JavaScript.
- Se puede renderizar tanto del lado del cliente como del servidor.
- Emplea un flujo unidireccional de datos y eso permite que se más predecible la aplicación y hay un seguimiento de los cambios. 

2. Definir qué es un componente en ReactJS y mencionar los tipos de componentes que existen.
R//: 
Se entiende como una pieza fundamental, autónoma y reutilizable que genera un comportamiento de un fragmento de la UI.
Por otro lado existen dos principales tipos de componentes, componentes de funciones, el cual es más funcional y simple, además se trabaja con hooks y de clases, el cual ofrece un estado interno y unos métodos de ciclo de vida más tradicionales. 

3. ¿Qué es el Virtual DOM y cuál es su función en ReactJS?
R//: 
El virtual DOM es una representatión eficiente del DOM real en una apliación de React y se crea cada vez que hay un cambio. Este primero realiza una comparación y analiza cuáles cambios se actualizaron y React primero actualiza el virtual DOM antes que el DOM del navegador.

4. ¿Qué es JSX en ReactJS y porqué es importante?
R//:
Es una extensión de sintáxis que permite combinar Javascript con HTMl y ello propende a la creación de un código más legible y mantenible y con pocas posibilidades de errores.

5. ¿Qué es un Hook en ReactJS y cuál es su propósito?
R//:
Los hooks son funciones especiales que permiten a los componentes tener estados, de igual manera, posibilita tener una mejor flexibilidad, reutilización del código y una forma más óptima de manejar el estado.

6. Mencionar al menos tres tipos de Hooks en ReactJS y explicar brevemente para qué se 
utilizan.
R//:
- UseEffect: es un hook de React que permite realizar efectos secundarios a componentes funcionales. Es utilizado para la actualización del estado, la llegada de nuevas props o el ciclo de vida de un componente.

- UseState: es un hook de React que es utilizado para declarar variables de estado en componentes funcionales y esto conlleva a un control y actualización del estado interno. 

- UseContext: es un hook de React que posibilita acceder al contexto de un componente funcional. Además es una forma sencilla de acceder a información sin tenerla que pasar manualmente de componente a componente. 

7. ¿Cuáles son las reglas de uso para los Hooks en ReactJS?
R//:
Para asegurar un óptimo funcionamiento con los hooks en React se deben seguir unas reglas,como por ejemplo: deben ser usados en componentes funcionales, no se debe usar los hooks fuera de los componentes de React, no llamar los hooks dentro de bucles,funciones anidadas, condiciones, etc. 

8. Explicar qué es React Router DOM versión 6, para qué se utiliza y cuáles son sus 
principales componentes y Hooks.
R//:
React Router DOM 6 es la librería más popular para la gestión de rutas en un proyecto de React. Permite que los componentes de React se muestren y oculten según la URL actual del navegador. Sus principales componentes son: 
- BrowserRouter: permite que interactúe con el historial del navegador y las URL y envuelve toda la apliación. 
- Routes: se utiliza para definir las rutas individuales y cómo se corresponden con los componentes.
- Route: representa una ruta de los componentes que deben renderizarse, path y element son propiedades importantes de este componente ya que ayudan a definir las rutas que deben mostrarse. 

Los hooks principalmente usados son: 
- useParams: permite acceder a los parámetros de la URL.
- useLocation: permite acceder a la información sobre la ubicación actual en tu aplicación React, además se puede obtener información detallada sobre la URL actual en un componente funcional.
- useNavigate:permite realizar redirecciones o cambios de ruta dentro de los componentes funcionales.

9. Explicar cómo se realiza la navegación entre diferentes páginas utilizando React Router DOM.
R//: 
- Instalar la librería react-router-dom.
npm install react-router-dom
- Configuración de las rutas (BrowserRouter, Routes, Route)
- Creación de enlaces mediante Link o NavLink
- Utilizar hooks para realizar navegaciones. 

10. ¿Cómo se definen rutas en React Router DOM?
R//: 
En Reat Router Dom las rutas se definen empleando Route y Routes y se utilizan dentro de BrowserRouter o Router.

11. Describir cómo crear un proyecto ReactJS con Vite
R//: 
Se introdue el comando con el que se inicia el poryecto
- npm create vite@latest my-vue-app -- --template react

Después de creado se instalan dependencia
- npm install 

Para ponerlo a correr
- npm run dev

12. Describir cómo desplegar un JSON server en cualquier Hosting free o servicio en la nube gratuito de su elección
R//: 
Se debe crear primeramente un JSON server de manera local, con los comandos que ello implica para crear y poner a correr el JSON Server. Luego en el archivo index.js se hacen unas sustituciones, igualmente que en el package.json,posteriormente se sube a un repositorio y luego se hace el hosting del JSON en las páginas que permiten hacerlo. 

13. Describir cómo desplegar una aplicación en cualquier Hosting de su elección. 
R//: 
- Se prepara el repositorio en Github
- Se elige el hosting, en este caso, Render
- Se crea una cuenta en Render y se inicia sesión
- Se le da en el botón azul "NEW", se despliegan varias opciones y se elige "WEB SERVICE"
- Se elige esta opción "Build and deploy from a Git repository" y se le da "NEXT"
- Se abre el Github y se selecciona el repositorio deseado
- Se configura el "NAME"
- Posteriormente se le da en la opción "CREATE WEB SERVICE" y queda desplegado. 

*MÓDULO SOBRE GESTION DE ESTADOS Y DATOS CON REACT CONTEXT Y USEREDUCER*

# Preguntas teóricas

1. ¿Qué es React Context y para qué se utiliza en el desarrollo web con React?
R//:
React Context es una característica de React que se utiliza para compartir datos sin tener que pasar props.

2. Describir cómo se crea un contexto en React y cómo se proporciona y consume información a través de él.
R//:
Se crea el contexto empleando useContext, el valor se provee a través del componente Provider y se consume con useContext y se evita pasar props manualmente a cada componente y facilitando el acceso a información 

3. ¿Cuál es la ventaja de utilizar React Context en lugar de pasar props a través de múltiples componentes?
R//:
La ventaja de utilizar React Context hace que el flujo de datos entre componentes sea más limpio, eficiente y legible, evitando el "props drilling", es decir, pasar props manualmente a través de varios componentes.

4. Explicar el propósito de useReducer en React y cómo se diferencia de useState.
R//:
Estos dos hooks, a grandes rasgos, se utilizan para gestionar el estado de los componentes, useReducer es para gestionar estados más complejos, mientras que useState es para estados más simples. UseReducer puede ser más apropiado si se piensa en legibilidad y mantenibilidad del código cuando el estado tiene una estructura compleja. UseState es ideal para estados simples en componentes funcionales, almacenando así un único valor de estado y una función para actualizar ese valor.

5. Describe los argumentos que toma la función useReducer.
R//:
Los argumentos que toma la función useReducer son:
- función reducer: es especifica cómo el estado de la aplicación cambia en respuesta a las acciones. 
- Initial State: es como ese punto de partido que se le da al estado cuando se inicia
- Init Function (Opcional): se utiliza para calcular el estado inicial de manera específica.

6. ¿Por qué es útil utilizar useReducer para gestionar el estado en aplicaciones más complejas?
R//:
Es útil utilzar useReducer, porque organiza de manera más eficiente el código, permite trabajar con estados más complejos, posibilita una separación importante en la lógica y también, por otro lado, por el tema de la escalabilidad, ya que permite adaptarse, crecer y sin perder el rumbo de su eficiencia y rendimiento.

7. ¿Cómo se puede utilizar React Context junto con useReducer para gestionar el estado global en una aplicación de React?
R//:
- Primero, se define un contexto usando React.createContext()
- Establecer el reducer
- Definir el proveedor
- Utilizar el contexto en componentes
- Consumir el estado global

8. ¿Por qué es importante tener un sistema de gestión de estado global en aplicaciones React más grandes?
R//:
- Mantiene el estado en un solo lugar
- Facilita compartir datos
- Mejora e rendimiento en general
- Permite la persistencia del estado
- Simplifica el mantenimiento

9. Menciona al menos tres ventajas de utilizar una combinación de React Context y useReducer en comparación con el manejo de estado local en componentes.
R//:
- Centralización del estado y la lógica
- Escalabilidad y el rendimiento
- Posibilita que el estado sea compartido globalmente

10. ¿En qué situaciones podría ser beneficioso migrar de un enfoque de manejo de estado local a un enfoque de estado global utilizando React Context y useReducer?
R//:
- Complejidad en la lógica
- Evita prop drilling 
- Necesidad de escalabilidad
- Compartir datos entre componentes



