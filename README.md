# react-book

http://apimeme.com/?ref=apilist.fun
https://randomuser.me/documentation#intro
https://jsonplaceholder.typicode.com/guide/


https://www.javascriptstuff.com/component-communication/
https://www.freecodecamp.org/news/how-to-clone-an-array-in-javascript-1d3183468f6a/

https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets

Componentes: Objeto (instancia)
<Item key="1" prop1="value1" prop2="value2"/>
- propiedades

Componente: Clase (en Visual estudio pongan rcc y te lo arma solito)

class Item extends React.Component /*algo asi como java.lang.Object*/ {
 constructor(props) {
 	super(props);
 		
 }
 
 render() { //representacion visual del componente. Algo asi como el toString();
 	return(<> JSX aca  </>);
 }
}
export default Item;

JSX: HTML dentro de javascript
return(
	<div>Hola Mundo!</div>
);

Reactiva: A partir del cambio de estado se redibuja (se vuelve a ejecutar render())

- Instalar VS Code
-- Instalar Find-Preferences-Extensions ES7 React/Redux/GraphQL/React-Native
- Prettier - Code formatter
-- en Settings, ponerlo como default formmater
-- poner Format on save = true

- instalar npm
- npm cache verify (si tenes error de integrity)
- npm install -g npm (para actualizar npm)

- npx create-react-app tpX

- npm install react-bootstrap bootstrap
After install, 
{/* The following line can be included in your src/index.js or App.js file*/}

import 'bootstrap/dist/css/bootstrap.min.css';

Importante: En un componentDidUpdate, puedo usar el this.setState()... pero ojo porque si no pongo una condicion de fin, genera un bucle infinito. Algo asi deberia tener: 
    if (previousProps.valor !== this.props.valor) { ... }

Forms: https://es.reactjs.org/docs/forms.html


https://es.reactjs.org/docs/thinking-in-react.html
(single resposibility principle)


- Instalar miktex
- Usar el pdflatex de miktex
- Instalar (tengo ubuntu 20), python3-pygments
- sudo apt install python3-pip
- pip3 install jsx-lexer (para JSX)
- run: (para usar minted 
/home/enrique/bin/pdflatex -shell-escape react-book.tex
- toque el lexer de javascript para agregar cuestiones de react con colores (javascript.py)

sudo mv /usr/lib/python3/dist-packages/pygments/lexers/javascript.py /usr/lib/python3/dist-packages/pygments/lexers/javascript.original.py

sudo gedit /usr/lib/python3/dist-packages/pygments/lexers/javascript.py 
-- si quiero agregar keywords para que las coloree
-- luego cambiamos el lenguage de block de mint, de jsx a cualquier otro, html por ejemplo y luego lo volvemos a cambiar.

-Cree un archivo enrique.py copia de friendly.py para cambiar colores
-sudo gedit /usr/lib/python3/dist-packages/pygments/styles/enrique.py
-sudo nano enrique.py //esta backapeado...

https://www.overleaf.com/learn/latex/Code_Highlighting_with_minted

- Very Basic required Javacript
- Core Concepts
-- Blog and Why I love React
-- Class based Componets
-- Function based Componets
-- Instantiation
-- props
-- state

-- Countdown


-- Hooks (Countdown with hooks)
-- Forms
-- 
-- HOC, aka Decorator pattern
-- Headless components
-- Duplicated Code (Visible)
--- duplicated code? => make another abstraction
- Example Apps
-- Dice
-- Layout with XX
-- Table (sorter and filters)



Esto es una prueba de otros colores...

\begin{listing}[H]
\title{bla/example.js}
\begin{minted}[fontseries=mc,
  		frame=lines,
               framesep=2mm]{jsx}
import React, { Component } from 'react';

export default class HelloMessage extends React.Component {
  //esto es un comentario...
  constructor(props) {
    super(props);
    let variable = "abc";
    this.state = {
      theme: true,
    };

  componentDidCatch() {
    let va = "asdf";
  }

    this.toggleTheme = () => {
      this.setState((state) => ({
        theme: state.theme === themes.dark,
      }));
    };
  }
    
  render() {
    return (
      <div>Hello {this.props.name}</div>
    );
  }
}

ReactDOM.render(
  <HelloMessage name="Taylor" />,
  document.getElementById('hello-example')
);
\end{minted}
\end{listing}


%chat
https://medium.com/@awaisshaikh94/chat-component-built-with-react-and-material-ui-c2b0d9ccc491
https://hapi.dev/tutorials/?lang=en_US




# guia-react
