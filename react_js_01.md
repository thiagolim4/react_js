# React JS 01

## Preparação de Ambiente
- Download do NodeJS (versão 10.15.3), utilizamos o mesmo como interpretador
- Qual a diferença entre o npm e o npx?
 - npm é gerenciador de pacotes, compartilha código Javascript
 - npx é o executador, package runner do npm
- Utilizar o create-react-app do facebook
- Ir na pasta desejada pro projeto:
```
npm install create-react-app
```
- npx: package runner do npm
```
npx create-react-app projeto-react
cd projeto-react
npm start
```
- Abre o projeto no navegador ```localhost:3000```

## Overview
- ```index.html```: código normal de página web, com div com ```id = root```
- ```App.js```: possui o que será renderizado dentro do elemento em index
- ```index.js```: renderiza, tem um DOM que está renderizando um App = ```App.js``` (tudo que está dentro dele), dentro de um elemento com uma ID ```root``` = ```document.getElementById('root')```

## Componentes
- Transformar a tabela em um componente
- Cria um ```Tabela.js```
```Javascript
class Tabela extends Component{
    render(){
      return(

      );
    }
}
export default Tabela;
```
- Para "componentizar" outro elemento dentro da própria tabela que é um elemento:
```Javascript
const TableHead = () => {
  return (

  );
}
```
- E depois para chamar dentro da própria tabela:
```Javascript
  <TableHead />
```
- Para passar informações de um componente para outro utiliza as chamadas ```props```: cria uma propriedade com um nome que quer e passa um valor para ela
- Dentro do render cria uma variável
- Key serve para o React saber qual elemento está modificando
- State trata dos estados do elemento
- State: Serve para guardar valores/estado que podem vir a mudar com a interação do usuário com o componente, tendo efeito na renderização do mesmo, o state pode ser passado como props!
- Props: Valores para a configuração de um componente, essas props são passadas pelo elemento acima (que utiliza o componente que irá receber) e são imutáveis, utilizado para a comunicação de componentes
