mesmo tendo um certo conhecimento de classes de outras linguagens
vou optar por seguir a ordem logica do roadmap que estou me baseando
até então ainda passei pelo conteudo de classes propriamente dito,
então vou seguir com a criação de objetos

```bash
const personagem = {
    nome: personagem1, // futura logica de escolha de nome 
    viada: 100,        // vida escala com o nivel 
    nivel: 1,          // sistema de ganho de xp
    
    ataque(){
        console.log("ataque") // futuro metodo de ataque
    },

    defesa(){
        console.log("defendeu") // logica de defesa baseada em status base de defesa - atk inimigo.
    },

    inventario: [] // 
}
```

sistema de armas separada do personagem. Funcionaria como uma especie de arsenal
o players teria a opção de escolher qual arma ele quer iniciar, cada arma teria seus
beneficios.

```bash
const armas = {
    espada: {},
    arco: {},
    machado: {}

    /* cada arma tera seu metodo de ataque proprio com uma logica por tras, por exemplo: espada recebe bonus de +2 de attk etc... */
}
```

logica semelhante ao arsenal de armas. Cada raça vai ter suas propriedades
unicas, talvez mais pro futuras metodos de atks proprios tambem, tipo poderes
de classes ou algo do tipo.

```bash
const racas = {
    humano: {},
    elfo: {},
    anao: {}

    /* a ideia e seguir sistemas de RPG que ja existem para ter um base já consolida,
    como implementaçoes futuras de subclasses tipo elfo negro, elfo da floresta, etc */
}
```

aqui seguirei o padrão dos outros objetos(futuras class), onde cada classe tera suas caracteristicas
proprias.

```bash
const classes = {
    barbaro: {},
    mago: {},
    bardo: {}
}
```

o sistema de xp vou apenas descrever como vou tentar fazer fazer, pois ainda não sei como
implementar. Pensei em fazer um contador que auentaria +1 sempre que o jogador derrotasse um inimigo,
caso ele não derrote o contador continuaria no mesmo lugar. Todo vez que o contator chegasse a 10 ele
resetaria e o nivel do jogador subiria em +1. Para aumentar a dificuldade conforme os leveis, a parti 
de um certo ponto por exemplo nivle: 10, para o jogar ganhar +1 no contador ele precisara matar X inimigos
ao invez de 1.

## Modelagem das Raças

A ideia inicial e trabalhar com 3 raças diferentes, onde cada raça dará um bônus especifico ao personagem do jogador. As 3 classes iniciais serão:

#### Humano

Humanos são a maioria na civilização atual do nosso mundo, eles possuem habilidades de arquitetura, possuem conhecimento de ervas medicinais e em alguns casos até conseguem usar magia, mas o diferencial deles está com certeza na incrível habilidade de causar confusão com as outras raças.

- Aptidão com todas as categorias de armas (pode usar qualquer arma)
- Bônus de vida(+150) de HP base
- habilidade: negociação — consegue negociar itens com mercadores por preços menores

#### Elfo

Diferente dos humanos, elfos são extremamente pacíficos ( com aqueles que respeitam as florestas ), dificilmente se envolvem em conflitos. Residem na arvore sagrada localizada no centro da maior floresta do continente, suas habilidades e conhecimentos sobre ervas medicinais e a natureza como todo e simplesmente indescritível.   

- Aptidão melhorada caso esteja usando um arco (+10 de dano) - não podem usar machado
- Bônus de mana (+50) base, caso esteja usando uma classe que possui mana
- habilidade: navegação — sempre conseguem achar seu caminho de volta

#### Anão

Habitantes tradicionais de grandes cidades escavadas dentro de montanhas. São mestres orgulhosos da mineração, da metalurgia e da engenharia, capazes de forjar as armas e armaduras mais resistentes

- Aptidão melhorada com martelo ( só pode usar martelo, porém todo dano e X2 )
- Bônus de vida(+50) e bônus de defesa(+10) em qualquer ação de defesa
- habilidade: ferreiro — pode aumentar a durabilidade de qualquer arma

