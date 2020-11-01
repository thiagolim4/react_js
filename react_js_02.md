# React JS 02

## Componentes
- Prettier: code formater para VS Code
- Plugin hightlight-selection para VS Code
- Simple React Snippets
- O default serve para podermos importar a classe sem precisar informar o nome dela entre {}, além de permitir mudar o nome da mesma durante a importação:
```Javascript
import UmaClasse from "TratadorErros";
import TratadorErros from "TratadorErros";

// evitando a necessidade de
import { TratadorErros } from "TratadorErros";
```

## Estilo
- Quando percorrer array (utilizando map ou forEach), pode colocar a prop key nos itens dentro das próprias tags
```Javascript
Array.of("Trabalho", "Estudos").map((item, index) => {
  return (
  <li key={index}>
    <p>{item}</p>
  </li>
  );
})
```
- Importar o arquivo css é só colocar o caminho dele
- Pode usar reset.css para deixar página em branco e poder aplicar os estilos
- Pode usar uma index.js dentro de uma pasta que tem um componente como um "índice" de aliases (apelidos), do tipo:
```Javascript
import CardNota from "./CardNota"
export default CardNota;
```
- Nesse caso CardNota é substituído pelo caminho quando usado
