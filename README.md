# LetMeAsk

Site desenvolvido durante a Next Level Week da Rocketseat <https://app.rocketseat.com.br/node/mission-react-js>
####
<a href="https://letmeask-b0622.web.app/">![image](https://user-images.githubusercontent.com/48057126/131685794-1c95f6a4-dcd5-49bc-9b8d-983f955babdf.png)</a>

## 🚀 Tecnologias

<ul>
  <li>HTML</li>
  <li>Typescript (TSX)</li>
  <li>SCSS</li>
  <li>React</li>
  <li>Realtime Database (Firebase)</li>
</ul>

## 💻 Objetivo

Este é um website desenvolvido para estudo inicial do React, aplicando diversos conceitos da tecnologia.

## 📚 Features

### ◼️ TSX

O TSX é um extensão de síntaxe para o Typescript, adicionando a possibilidade de construção UI inicial da página dentro do Typescript.

```tsx
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
ReactDOM.render(
  element,
  document.getElementById('root')
); //Exemplo retirado da documentação do React (https://pt-br.reactjs.org/docs/introducing-jsx.html)
```
  Como podemos observar no exemplo, há a declaração da constante "name" que, em seguida, é utilizada no TSX dentro de chaves. Você poderia inserir qualquer expressão do Typescript no lugar de "name". Desta forma, a lógica de renderização e o desenvolvimento UI estão agregados, além disso, a separação de conceitos é realizada através da produção de Componentes React. Uma característica do JSX e TSX é a utilização do camelCase nos nomes das propriedades, assim, "class" deve ser escrita "className", "tabindex" deve ser "tabIndex" e entre outras.

### ◼️ React Components

Segundo a documentação oficial do React, os componentes, são como funções Javascript, podem receber entradas (denominadas "props") e retornam elementos React. A sua principal utilidade é justamente essa capacidade de dividir a UI em partes isoladas e retornando estes elementos, deste modo, permitindo a sua reutilização em diferentes momentos do código. Além das "props" os componentes podem ser estilizados individualmente. <br><br>Abaixo temos o exemplo de um componente Button, que pode, ou não, receber a class 'outlined' (para aplicar, ou não, determinada estilização), através da prop "isOutlined", que serve como condição para tal , além de que, este componente recebe como props, em conjunto da "isOutlined", os atributos de um "button" do HTML.

```tsx
import { ButtonHTMLAttributes } from 'react';

import './styles.scss';

type ButtonProps = ButtonHTMLAttributes<HTMLButtonElement> & {
  isOutlined?: boolean
};

export function Button({ isOutlined = false, ...props }: ButtonProps){
  return(
    <button className={`button ${isOutlined ? 'outlined' : ''}`}
      {...props}
    />
  )
}
```

### ◼️ React Hooks

Os hooks permitem a utilização de diversos recursos do React como o state, o effect e de criação própria, sem a necessidade da criação de classes para tal. No exemplo abaixo, temos a criação de um hook denominado UseAuth, que utiliza um contexto, de criação própria, denominado AuthContext e o hook useContext do react, podendo ser utilizado no código para a autenticação dos usuários.
```js
import { useContext } from "react";
import { AuthContext } from "../contexts/AuthContext";

export function useAuth() {
  const value = useContext(AuthContext);
  return value;
}
```

### ◼️ Além disso, apresenta responsividade para os diversos dispositivos e utiliza os serviços de banco de dados e hosting do Firebase

![image](https://user-images.githubusercontent.com/48057126/131711105-36f1a79e-befb-49e6-8626-f6abd4f845ca.png)
