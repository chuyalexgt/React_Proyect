## React

 - **Herramientas necesarias**
 
 - [ ] chrome
 - [ ] Reactt developers tools
 - [ ] visual studio code
 - [ ]  Extension *Prettier* en VSC
## Iniciar un proyecto
 - instalar de forma global desde npm el ***create-react-app***
 `npm install -g create-react-app`
 
 - Desde la terminal y dentro de la carpeta donde quieras guardar tu proyecto corre el siguiente comando
 `create-react-app nombre-del-proyecto`
 - Correr el comando ***npm run start*** dentro de la carpeta creada por react.

## Trabajando en src/index.js
Para trabajar con react en cualquier script necesitamos importar las siguientes dos librerias:
**Siempre que tu codigo tenga jsx debes importar react**
 - `import React from "react"`
 - `import ReactDOM from "react-dom"`
 - List item

***Renderizar etiquetas en react***
```javascript
const  element = <h1>Hello, Platzi Badges!</h1>;
const  container = document.getElementById('app');
// ReactDOM.render(__qué__, __dónde__);
ReactDOM.render(element,container)
``` 
***Crear elementos con react (no se usa, es mejor con jsx)***
```javascript
const element = createElement("h1",{},"hola soy juanito")
// const nombre_elemento = createElement("tipo_elemento",{props}, "childrens")
```

***Crear elementos con JSX*** 
```jsx
const element = (
	<div>
		<h1> HOLA </h1>
		<p> soy un gato :3 </p>
		<p> {//cualquier cosa de js se pone entre corchetes} </p>
	</div>
)
```
Como puedes ver, trabajar con JSX es mucho mas facil, ademas de que nos permite crear conjuntos de elementos a los que llamaremos componetes

***Componetes***
Se pueden entender como piezas de lego que juntas sirven para armar un sin fin de cosas, o en este caso, construir un website, lo que hicimos en el ejemplo anterior, es un componente, y lo mejos es hacerlos lo mas genericos posibles, de este modo podemos reutilizarlos en otros proyectos.

La relación componente / elemento puede ser vista como la relación clase/objeto en la POO, un componente sería el plano y un elemento seria lo que creas con ese plano.

***Identificación de componetes***
Necesitas dos preguntas guia:

 1. ¿Qué elementos se repiten?
 2. ¿Qué elementos cumplen una función muy específica?
