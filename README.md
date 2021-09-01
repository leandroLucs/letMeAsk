# LetMeAsk

Site desenvolvido durante a Next Level Week da Rocketseat
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

O TSX é um extensão de síntaxe para o Typescript, adicionando a possibilidade de construção UI inicial da página dentro do Typescript
```tsx
const element = <h1>Hello, world!</h1>; //Exemplo retirado da documentação do React (https://pt-br.reactjs.org/docs/introducing-jsx.html)
```

####

### ◼️ Biblioteca Swiper para exibição dos meus trabalhos em Portifólio

![image](https://user-images.githubusercontent.com/48057126/131558013-20584811-ddc7-459b-b374-a4bd641dc480.png)

####

### ◼️ Biblioteca Scroll Reveal para exibição dos itens gradualmente de forma suave, com uma pequena transição

```js
const scrollReveal = ScrollReveal({
  origin: 'top',
  distance: '30px',
  duration: 700,
  reset: true
})

scrollReveal.reveal(
  `#home .text, #home .scroll-down,
  #about .title, #about .bio, #about .paragraph-1, #about .paragraph-2,
  #portfolio .text, .swiper-container,
  #contact .text, #contact .links, #contact form
  `,
  { interval: 100 }
)
```
### ◼️ Envio de E-mail com o PHPMailer
![image](https://user-images.githubusercontent.com/48057126/131681864-b294b329-9838-469e-ae3a-3e7152c63d6b.png)


### ◼️ Além disso, apresenta responsividade para os diversos dispositivos

![image](https://user-images.githubusercontent.com/48057126/131559653-3b12b7f1-46bf-4842-a236-cf76ecad0665.png)
