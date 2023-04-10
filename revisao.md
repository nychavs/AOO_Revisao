# Analise orientada a objetos 
## Objetivo da disciplina:
> Conhecer e aplicar técninas para levantamento de especificação de requisitos, modelagem estrutural e comportamento de sistemas orientados a objeto.

### Paradigmas
- Estruturado: apenas processos e dados;
- Orientado: modelagem do conjunto de fatos/conceitos associados ao problema, o tratamento desse problema deve ignorar tanto quanto possível a existencia do mundo computacional

*a diferença de analise de projeto e de projeto da solução é basicamente que o primeior vai enfatizar uma investiação do problema ao invés da solução, já o segundo enfatiza uma solução conceitual em software/hardware*

### Vantagens da modelagem orientada a objetos
 - descrição mais facilmente compreensível;
 - proporciona diferentes pontos de vista;
 - baixo nivel de asbtração;
 
 ### Conceitos
 - Encapsulamento:
 restringir o acesso ao comportamento de um objeto, como forma de proteção, controlando as operações realizadas com/por um objeto.

- Polimorfismo:
os mesmos atributos podem ser usados em objetos diferentes com lógicas diferentes, também indica a capacidade de abastrair varias implementações diferentes em uma unica interface

- Herança:
classes semelhantes são agrupados em uma unica classe mais generalizada (ex: animal <- mamifero <- gato) cada uma das classes herdadas possuem as caracteristicas e comportamentos da classe mae/pai

## Diagrama de caso de uso
Apresenta uma visão externa das funcionalidades que o sistemas possuirá e sua relação com os usuários de forma delimitada.

Atores
> são papeis desempenhados por usuarios de um sistema, estimulam/solicitam ações/eventos do sistema e recebem retorno. Exemplos para ajudar na identificação:
> - quem usa o sistema?
> - quem inicializa o sistema?
> - quem fornece os dados?
> - quem usa as informações?
nunca utilizar o nome do ator! muito menos "sistema", preferivel: usuário, administrador (função)

Casos de uso
> representa os principais comportamentos (serviços tarefas, funcionlidades) do sistema observaveis pro um ator, descrevendo o que um sistema deve conter. Ex: Nome no infinitivo + objeto (cadastro de usuario para comprar carros)

### Conceitos
- Associações:
representam as interações ou relacionamentos
entre os atores que fazem parte do diagrama

- Generalização/Especialização:
Usado quando existem dois ou mais atores/casos de uso com características semelhantes, apresentando pequenas diferenças entre si. Ex: uma pessoa fisica e uma pessoa juridica são pessoas.

- Inclusão/Include:
usado quando existe uma situaçao que se repete para mais de um caso de uso, quando essa relação é feita obrigatoriamente ela será executada. nesse caso a seta aponta para o que será incluido.

- Extensão/Extend:
diferentemente do include, as extensões não obrigatoriamente acontecem e a seta aponta para a classe mae

## Diagrama de classe
Apresentam as entidades (classes) que compoe o sistema, os dados (atributos), o comportamento delas (metodos) e como se relacionam (associações)

Associações
> as possiveis associações são 1, 0..1, 1..*, 0..*, ou até mesmo a multiplicidade, onde é dado um numero especifico (ex: 4) x..y
> as associações podem possuir papeis, ex: dono possui propriedade, onde dono vem de uma classe e propriedade de outra

Agregações
- indica uma relação de todo-parte, ex: equipe <>--- jogador (equipe é o todo e o jogador é a parte), no caso o objeto contido pode existir sem o que o ontem, então o jogador pode existir sem a equipe. Nesse caso o losango não é pintado.

Composição
- diferentemente da agregação, nesse caso a parte do todo nao pode existir sem o todo, ex: pessoa e cpf, nao existe cpf sem a pessoa existir. a diferença na ligação é que o losango será todo pintado
