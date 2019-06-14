![alt text](http://www.viajarbarato.com.br/images/challenge/logo-vb.png)

# Desafio para candidatos à vaga de desenvolvedor (Vaga Presencial)
A ideia deste desafio é nos permitir avaliar melhor as habilidades de candidatos à vagas de programador, de vários níveis.
Este desafio deve ser feito por você em sua casa. Gaste o tempo que você quiser, porém normalmente você não deve precisar de mais do que algumas horas.
> Este é um desafio com vaga em aberto qualquer um pode participar.

## Instruções de entrega do desafio
1. Primeiro, faça um fork deste projeto para sua conta no GitHub (crie uma se você não possuir).
2. Em seguida, implemente o projeto tal qual descrito abaixo, em seu próprio fork.
3. Crie as instruções de instalação e execução do aplicativo em seu `readme.md`.
4. Por fim, envie o link do seu repositório público para avaliarmos seu código para o e-mail [marco.faustino@viajarbarato.com.br](marco.faustino@viajarbarato.com.br)

## Dissertação sobre arquitetura de solução
Crie um arquivo `dissertacao.txt` na raiz do seu repositório, dentro deste arquivo você deve dissertar sobre o seguinte tema:

**Sabendo que todos os programadores do Viajar Barato possuem amplo conhecimento em .NET e SQL Server, se você fosse construir um novo site do Viajar Barato, qual tecnologia e arquitetura você usaria? Explique o motivo da sua escolha e aponte como usar cada uma delas.**

## Descrição do projeto prático.
- O desafio é criar tanto uma API REST quanto uma página SPA em Angular@5+ que lista os personagens da série de filmes "Star Wars" filtrando por sua espécie.

- Você deve criar uma WEB API RESTFull utilizando C# que irá consumir os métodos de [https://swapi.co/](https://swapi.co/documentation), você deve decidir com base nas necessidades do software e documentação do [https://swapi.co/](https://swapi.co/documentation) quais métodos serão necessários o encapsulamento.

- Você deve criar uma Página utilizando Angular@5+, React ou MVC, que será responsável por efetuar a busca de personagens e listar os nomes dos personagens de uma determinada espécie.

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
* No filtro de espécies utilizar um componente de Typeahead;
* Utilizar .Net Framework 4+ ou .NET Core 1.1+;
* Utilizar Angular@5+, React ou MVC;
* Pode utilizar [@ng-bootstrap/ng-bootstrap](https://ng-bootstrap.github.io/) ou [Angular Material](https://material.angular.io/);
* Pode utilizar [IdentityServer4](http://docs.identityserver.io/en/latest/);
* Deve implementar autorização na API, baseada em Tokens com expiração;

## Sua aplicação NÃO DEVE:
* Importar pacotes de auxílio do swapi.co.
* Acessar a swapi.co diretamente via interface client.

## Quer mostrar mais de seu potencial:
* Faça uso correto da programação paralela;
* Efetue uma implementação de Cache;
* Siga os conceitos de OOP e SOLID;
* Utilize ao menos duas das design patterns da OOP;
* Efetue commits atômicos;
* Inclua documentação por comentários;
* Utilize dutos assíncronos;
* Implemente o conceito de dutos em suas subscrições;
* Utilize quando necessário a composição de mapaeamento ou troca de mapeamento;
* Autenticar o acesso aos métodos anônimos da aplicação Angular ao Backend C# utilizado OAuth2 Client credentials;

## Conhecimentos que procuramos no candidato: 
* Desenvolvimento orientado a objeto 
* C# 5+
* .NET Framework 4+
* Integrações RESTFull
* HTML 
* CSS 
* Pré-processadores de Estilo
* Javascript
* ASP.net MVC (Razor Engine) 
* Banco de dados SQL Server 
* Git Source Control 
* Desenvolvimento orientado a testes (TDD) 

## Conhecimentos do candidato que fazem a diferença: 
* C# Async Framework 
* Entity Framework Core
* .NET Core 2 ou superior 
* Angular 5+
* Typescript 3+ 
* Docker 
* Banco de dados não relacional MongoDB 
* AMQP RabbitMQ – Queues
* Banco de dados não relacional Redis
* Programação Reativa
* Linux
* Kubernetes
* Continuous integration e continuous delivery (CI/CD) 

## Avaliação
Seu projeto será avaliado de acordo com os seguintes critérios. 

1. Sua aplicação atende funcionalmente o que foi pedido;
2. Você foi conciso em sua dissertação apontando pontos interessantes e com uma visão disruptiva.
3. Você documentou a maneira de configurar o ambiente e rodar sua aplicação na máquina do avaliador utilizando o README.md;
4. Você seguiu as instruções enviadas;
5. Você segue as boas práticas de programação e entrega para o Cliente;
6. O código escrito é fácil de entender e manter;
7. Você se preocupa com o uso do aplicativo pelo Usuário;
8. Você executou o teste em um prazo máximo de 9 dias a contar da data do fork.

> Tentaremos verificar a sua familiarização com as bibliotecas padrões (standard libs), bem como sua experiência com programação orientada a objetos a partir da estrutura de seu projeto, preocupação com o objetivo da aplicação e do seu uso pelo usuário, suporte e manutenção do código por outros desenvolvedores.

### Processo de feedback do teste
Após a entrega do link do códido fonte do projeto no GitHub, efetuaremos a análise da entrega, normalmente em até 36 horas úteis teremos o resultado da análise.

Em caso positivo será iniciada a segunda faze de avaliação onde acontecerá uma entrevista com a equipe, onde o candidato irá apresentar o projeto que construiu e detalhar quais técnicas ele utilizou e porque.

Caso haja necessidade agendaremos uma entrevista presencial.

## Um pouco mais de como é trabalhar com a gente
Somos uma empresa de turismo com mais de 7 anos de atuação.

Estamos em processo de modernização de nossa Stack de desenvolvimento, implementando arquiteturas escaláveis utilizando containers e micro-serviços.

Fazem parte de nossa Stack: .NET Core 2+, .NET Framework 4+, Angular@5+, RabbitMQ, Docker, Kubernetes, Linux, MongoDB, MSSql Server, Typescript.

Apoiamos e respeitamos a diversidade independente de raça, etnia, orientação sexual, gênero, idade, nacionalidade, crença ou deficiência.

### Localização
Estamos localizados no centro de São Paulo proximo a nós temos: 
* :station: Metrô Sé, Anhangabaú e São Bento. 
* :computer: Rua Santa Ifigênia
* :metal: Galeria do Rock
* :hamburger: Shopping Light 

**Venha! Junte-se a nós!**
:airplane::heart_eyes::coffee::computer::headphones::hocho::skull: