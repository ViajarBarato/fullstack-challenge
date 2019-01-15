![alt text](http://www.viajarbarato.com.br/images/challenge/logo-vb.png)

# Desafio para candidatos à vaga de desenvolvedor Full Stack
A ideia deste desafio é nos permitir avaliar melhor as habilidades de candidatos à vagas de programador, de vários níveis.
Este desafio deve ser feito por você em sua casa. Gaste o tempo que você quiser, porém normalmente você não deve precisar de mais do que algumas horas.

## Instruções de entrega do desafio
1. Primeiro, faça um fork deste projeto para sua conta no GitHub (crie uma se você não possuir).
2. Em seguida, implemente o projeto tal qual descrito abaixo, em seu próprio fork.
3. Crie as instruções de instalação e execução do aplicativo em seu `readme.md`.
4. Por fim, envie o link do seu repositório para avaliarmos seu código.

## Dissertação sobre arquitetura de solução
Crie um arquivo `dissertacao.txt` na raiz do seu repositório, dentro deste arquivo você deve dissertar sobre o seguinte tema:

**Sabendo que todos os programadores do Viajar Barato possuem amplo conhecimento em .NET e SQL Server, se você fosse construir um novo site do Viajar Barato, qual tecnologia e arquitetura você usaria? Explique o motivo da sua escolha e aponte como usar cada uma delas.**

## Descrição do projeto prático.
- O desafio é criar tanto uma API REST quanto uma página SPA em Angular@5+ que lista os personagens da série de filmes "Star Wars" filtrando por sua espécie.

- Você deve criar uma WEB API RESTFull utilizando C# que irá consumir os métodos de [https://swapi.co/](https://swapi.co/documentation), você deve decidir com base nas necessidades do software e documentação do [https://swapi.co/](https://swapi.co/documentation) quais métodos serão necessários o encapsulamento.

- Você deve criar uma Página utilizando Angular@5+, que será responsável por efetuar a busca de personagens e listar os nomes dos personagens se uma terminada espécie.

- O Filtro de busca da página será composto por um campo onde o usuário irá digitar a espécie, esse campo deve ser do tipo typeahead search com uma pesquisa da esquerda para direita, onde conforme a digitação do usuário os termos compatíveis são exibidos em um Dropbox, os termos gerados no typeahead. Além de exibir do nome da espécie compatível com o termo o nome do planeta natal "homeworld.name" deve ser apresentado. 
**Exemplo**: *Usuário digita: `Hum` > Aplicação Apresenta: [`Human (Coruscant)`]*

- A Tabela de Resultado da busca "personagens", deve ser composto pelo nome do personagem e o nome do planeta natal "homeworld.name". Abaixo uma tabela com exemplo do retorno.

    | Personagem | Planeta Natal |
    | ------ | ------ |
    | Luke Skywalker | Tatooine |
    | Darth Vader | Tatooine |
    | Leia Organa | Alderaan |
    | Owen Lars | Tatooine |

> Os serviços de consulta de personagens, planetas e espécies e fornecido pelo The Star Wars API, a documentação pode ser acessada nesse link [https://swapi.co/documentation](https://swapi.co/documentation).

Abaixo um exemplo de como sua aplicação deve se parecer. `challenge-mock-wireframe.jpg`
![alt text](http://www.viajarbarato.com.br/images/challenge/challenge-mock-wireframe.jpg)

## Sua aplicação DEVE:
* Deve autenticar o acesso aos métodos anônimos da aplicação Angular ao Backend C# utilizado OAuth2 Client credentials;
* No filtro de espécies utilizar um componente de Typeahead;
* Utilizar .Net Framework 4+ ou .NET Core 1.1+;
* Utilizar Angular@5+;
* Pode utilizar [@ng-bootstrap/ng-bootstrap](https://ng-bootstrap.github.io/) ou [Angular Material](https://material.angular.io/);
* Pode utilizar [IdentityServer4](http://docs.identityserver.io/en/latest/);

## Sua aplicação NÃO DEVE:
* Não deve importar pacotes de auxílio do swapi.co.
* A página angular não deve acessar a swapi.co diretamente.

## Quer mostrar mais de seu potencial:
* Faça uso correto do System.Threading.Tasks;
* Efetue uma implementação de Cache;
* Siga os conceitos de OOP e SOLID;
* Utilize ao menos duas das design patterns da OOP;
* Efetue commits atômicos;
* Inclua documentação por comentários;
* Utilize AsyncPipe em sua página angular;
* Implemente o conceito de piping em suas subscrições;
* Utilize quando necessário o método switchMap;
* Implemente a paginação de itens com Observables;

## Avaliação
Seu projeto será avaliado de acordo com os seguintes critérios. 

1. Sua aplicação atende funcionalmente o que foi pedido;
2. Você foi conciso em sua dissertação apontando pontos interessantes e com uma visão disruptiva.
3. Você documentou a maneira de configurar o ambiente e rodar sua aplicação na máquina do avaliador utilizando o README.md;
4. Você seguiu as instruções enviadas;
5. Você segue as boas práticas de programação e entrega para o Cliente;
6. O código escrito é fácil de entender e manter;
7. Você se preocupa com o uso do aplicativo pelo Usuário;

> Tentaremos verificar a sua familiarização com as bibliotecas padrões (standard libs), bem como sua experiência com programação orientada a objetos a partir da estrutura de seu projeto, preocupação com o objetivo da aplicação e do seu uso pelo usuário, suporte e manutenção do código por outros desenvolvedores.
