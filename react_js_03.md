# React JS 03

## Propriedades
- ```evento.preventDefault()``` evita o comportamento padrão do componente
- ```evento.stopPropagation()``` impede a propagação do evento na árvore do DOM
- Um componente pai pode passar sua função como prop para os filhos, e esse filho vai executar a função do pai (como por exemplo, alterar lista de notas)
 - Inserir isso nos componentes filhos é considerado injeção de dependências
- Se no seu contrutor de classe não tem nenhum atributo além das props, o JavaScript já faz isso pra você automaticamente então nem precisa de construtor
- Propriedades passadas aos objetos são imutáveis (quando se recebe a props)

## State
- A cada alteração de uma variável dentro do State, ele chama o render() para colocar as alterações na página (primeiro faz no DOM, e depois aplica na página de verdade)

## SVG
- Pode importar como imagem normal, ou como uma tag:
```Javascript
import {ReactComponent as imagemSVG} from "../../assets/img/imagem.svg"
<imagemSVG/>
```

## Index
- Usando vetor no state, com o map, precisa do index para os itens. Passando esse index para os componentes abaixo (que você retorna), é possível, ao clicar em um item específico, pegar o index e deletar o elemento do vetor (do state).
