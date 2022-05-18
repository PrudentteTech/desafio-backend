# Desafio Prudentte - Backend

Obrigado pelo interesse em fazer parte no nosso time! Para participar do processo de seleção, é necessário que todos os interessados pela vaga façam esse desafio. 
Crie um repositório sem nenhuma referência à Prudentte e após a finalização, entre em contato com quem te contactou, notificando a finalização do desafio.

Se não entender algum conceito ou parte do problema, não é motivo para se preocupar! Queremos que faça o desafio até onde souber.

## O desafio

Contrua um uma API Rest em NodeJS para um encurtador de URL, que será consumida externamente. Não é necessário haver nenhum tipo autenticação

### Requisitos

Essa API deve conter:

**Rota para cadastro de url**

Exemplo de request:
```json
{
  "user_id": 1,
  "url": "https://www.google.com/",
  "expire_date": "2022-09-15"
}
```
Exemplo de response:
```json
{
  "user_id": 1,
  "url": "https://www.google.com/",
  "expire_date": "2022-09-15",
  "shortened_url": "https://short.com/{hash}"
}
```
**Rota para busca da url encurtada**

A resposta deve ser um redirecionamento para a rota cadastrada.

**Rota para buscar dados de uma url**

O response deve conter:
  - Data de cadastro
  - Número total de buscas pela url
  - Número de buscas pela url nos últimos 7 dias.


**Rota para buscar as urls cadastradas por 1 usuário**

Exemplo de response:
```json
[
  {
    "user_id": 1,
    "url": "https://www.google.com/",
    "expire_date": "2022-09-15",
    "shortened_url": "https://short.com/{hash}"
  }
]
```



### Importante

- Deve ser utilizado um banco de dados para a persistência dos dados.
- É necessário uma camada de cache distribuido nos endpoints de consulta.
- Se for utilizar um framework tente evitar usar muito métodos ou atalhos já prontos. Sabemos que essas facilidades aumentam a produtividade no dia-a-dia mas aqui queremos ver o seu código e a sua forma de resolver problemas.

## O Esperado

Além dos requisitos levantados acima, iremos olhar para os seguintes critérios durante a correção do desafio:

- Arquitetura (DDD, Clean Architecture)
- Documentação (comente sobre decisões técnicas, escolhas, etc)
- Testes (unitários, e2e, etc)
- Padrão de commits
- Cuidado com itens de segurança
- Código limpo e organizado
- Se for para vaga sênior, foque bastante no **desenho arquitetural**
- Docker Compose (para a utilização dos bancos de dados escolhidos)


## Diferencial

- Dockerfile
- Uso de design patterns
- Proposta de melhoria de architetura

## Entrevista Técnica

Na data marcada pelo recrutador tenha sua aplicação rodando na sua máquina local para execução dos testes e para nos mostrar os pontos desenvolvidos e possíveis questionamentos. 
Faremos um code review junto contigo como se você já fosse do nosso time, você poderá explicar o que você pensou, como arquitetou e como pode evoluir o projeto


Qualquer dúvida, entre em contato! Boa sorte 😄
