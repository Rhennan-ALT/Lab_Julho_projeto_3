## 21/07/2026

## Objetivo:

Criar a estrutura inicial do projeto.

Aprendizados:

- Organizar um projeto é tão importante quanto escrever código.
- Separar responsabilidades facilita o crescimento do sistema.

Dificuldades:

Ainda tenho dúvidas sobre como dividir alguns arquivos.

Próximo passo:

Criar a entidade Personagem.

## 21/07/2026

- preparativos do game-design inicial estabelecidos.
- finalização da construção inicial da estrutura.
- planejamento mental sobre o próximo passo: criação de personagem.

## 22/07/2026

## Decisão arquitetural

Hoje alterei completamente a forma como pensei a entidade Personagem.

Antes eu adicionava tudo que um personagem poderia possuir.

Agora passei a separar:

- O que o personagem É.
- O que o personagem TEM.

Essa mudança deixou a modelagem muito mais limpa e facilitará futuras expansões do projeto.

## 23/07/26

## Decisão de Arquitetura

Hoje foi decidido que:

- O personagem não conhecerá diretamente as armas.
- O personagem possuirá um inventário.
- O inventário armazenará os itens.
- Cada item será modelado separadamente para facilitar futuras expansões.

## 24/07/26

## Resumo do dia

O foco do estudo foi aprofundar o entendimento sobre Arrays aplicando os conceitos diretamente no desenvolvimento do Mini RPG.

Durante a parte teórica foram discutidos conceitos importantes sobre busca, armazenamento e manipulação de conjuntos de dados, sempre pensando primeiro na lógica antes da implementação em JavaScript.

Após o estudo teórico, os conceitos foram aplicados na arquitetura do projeto.

Implementações realizadas
Sistema de Inventário

Foi implementada a estrutura inicial do inventário utilizando um Array.

O inventário passou a armazenar objetos completos ao invés de valores simples, representando de forma mais fiel o funcionamento de um inventário em um jogo.

Exemplo:

- Espada Simples
- Arco Simples
- Espada Longa

Todos adicionados através de push().

## Modelagem das raças

Foi iniciada a modelagem do sistema de raças.

As três primeiras raças foram definidas:

- Humano
- Elfo
- Anão

Cada raça possui:

- id
- nome
- aptidão
- bônus
- habilidade especial

Neste momento as propriedades ainda funcionam como planejamento para futuras implementações.