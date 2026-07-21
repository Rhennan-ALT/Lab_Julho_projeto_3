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

