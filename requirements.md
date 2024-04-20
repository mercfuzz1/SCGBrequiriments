
---

<h1>Requisitos de Software</h1>

<h2>Sistema de consulta e gestão de boletos (SCGB)</h2>

<small>Versão 1.0</small>

---

## Histórico de revisões

|    Data    | Versão |          Descrição          |      Autor             |
| :--------: | :----: | :-------------------------: | :--------------:       |
| 17/04/2024 |  1.0   |    Criação do documento     | Daniel Cassemiro Alves |

---

## Sumário

- [Introdução](#introdução)
  - [Definições, Acrônimos e Abreviações](#definições-acrônimos-e-abreviações)
- [Usuários identificados](#usuários-identificados)
- [Requisitos funcionais](#requisitos-funcionais)
  - [Usabilidade](#Usabilidade(RF))
  - [Privacidade e segurança](#privacidade-e-segurança(RF))
- [Requisitos não-funcionais](#requisitos-não-funcionais)
  - [Usabilidade](#usabilidade(RNF))
  - [Privacidade e segurança](#privacidade-e-segurança(RNF))
  - [Suportabilidade](#suportabilidade)
  - [Manutenibilidade](#manutenibilidade)
- [Matriz de rastreabilidade](#matriz-de-rastreabilidade)
  - [Rastreabilidade entre NFs e RNFs](#rastreabilidade-entre-nfs-e-rnfs)

---

# Introdução

O objetivo deste documento é apresentar os requisitos de software do produto **Sistema de consulta e gestão de boletos (SCGB)**

## Definições, Acrônimos e Abreviações

Esta subseção fornece as definições de todos os termos, acrônimos e abreviações necessárias à adequada interpretação do Documento de Requisitos.

  O identificador do tipo de requisitos é conforme abaixo:

  - RF – Requisito Funcional
    - Requisito funcional é aquele essêncial para o funcionamento e operação do sistema.
  - RNF – Requisito Não-Funcional
    - Requisito não funcional é aquele que faz parte do contexto do funcionamento e operação do sistema mas não é essêncial.
  - RB - Possíveis requisitos Bônus/ futuros

  O identificador do requisito será uma sequência numérica. Esse número sequencial será único para todo o conjunto de tipos de requisitos.

  **Exemplo**: RF0001, RF1234, RNF1234,

  A matriz de rastreabilidade definirá a relação entre os requisitos funcionais e não funcionais.

# Usuários identificados

Os seguintes usuários foram identificados para o sistema:

- Usuário do sistema
  - Usuários comuns
    - Usuário cliente
  - Administrador do sistema

# Requisitos funcionais

## Usabilidade(RF)

- **[RF001]** - Como usuário, terei como acessar o sistema via login, por e-mail e senha.
- **[RF002]** - Como usuário poderei logar e deslogar do sistema com facilidade apartir de um uma seção de "bandeja" de usuário.
- **[RF003]** - Como cliente terei acesso à um dashboard próprio que me disponibilizará acesso à consulta de meus boletos, que serão listados em formato de tabelas entituladas pelo ano referente dos boletos, com os seguintes campos: descrição do boleto, tipo do boleto, data da criação do boleto, data de validade dos boletos, ações.
- **[RF004]** - Como cliente poderei baixar meus boletos a partir do campo de ações das tabelas de listagem de boletos. 
- **[RF005]** - Como administrador terei acesso à um dashboard próprio que me dará acesso à um seção única que disponibilizará as seguintes subseções: Informações Próprias(nome, cargo e ícone), Gerenciamento de clientes(visualizar,adicionar, remover ou atualizar).
- **[RF006]** - Como administrador poderei acessar as informações de quaisquer clientes na seção de gerenciamento de clientes e manipulá-las(visualizar,adicionar, remover ou atualizar).

## Privacidade e Segurança(RF)

- **[RF007]** - O sistema deve ser desenvolvido de forma que os dados dos clientes sejam protegidos e não sejam acessíveis por terceiros.
- **[RF008]** - O sistema deve ser desenvolvido de forma que os dados pessoais dos clientes sejam criptografados, como endereço de e-mail, senha, nome completo, cidade e estado.
- **[RF009]** - O sistema deve ser desenvolvido de forma que os usuários logados apenas consigam acessar as suas próprias rotas privadas.
- **[RF010]** - O sistema deve ser desenvolvido de forma que um usuário possa apenas visualizar determinada feature se tiver a devida permissão.
- **[RF011]** - o sistema deve ser desenvolvido de forma que os usuários possuam um login único.

# Requisitos não-funcionais

## Usabilidade(RNF)

- **[RNF001]** - Como cliente, no dashboard, poderei ver minhas informações próprias, sendo elas: nome, e-mail, data de início de contrato, data de validade do contrato, serviço contratado, logo da empresa.
- **[RNF002]** - Como cliente poderei ter a possibilidade de acessar o blog da VLTech com facilidade apartir de um botão de "retornar" por exemplo.

## Privacidade e Segurança(RNF)

- **[RNF003]** - Como usuário poderei ter a possibilidade de recuperar minha senha.

## Suportabilidade

- **[RNF004]** - O sistema deve ser desenvolvido de forma que possa ser executado nos três principais navegadores da web: Google Chrome, Mozilla Firefox e Microsoft Edge através de um computador com sistema operacional Windows, Linux ou Mac OS.

## Manutenibilidade

- **[RNF006]** - O sistema deve ser desenvolvido de forma que possa ser facilmente atualizado e mantido.

# Matriz de rastreabilidade

A matriz de rastreabilidade é apresentada a seguir.

## Rastreabilidade entre NFs e RNFs

| RF / RNF | RF001 | RF002 | RF003 | RF004 | RF005 | RF006 | RF007 | RF008 | RF009 | RF010 |
| :------: | :---: | :---: | :---: | :---: | :---: | ----- | ----- | ----- | ----- | ----- |
|  RNF001  |       |       |   X   |       |       |       |       |       |       |       |
|  RNF002  |       |       |       |       |       |       |       |       |       |       |
|  RNF003  |   X   |       |       |       |       |       |       |       |       |       |
|  RNF004  |       |       |       |       |       |       |       |       |       |       |
|  RNF005  |       |       |       |       |       |       |       |       |       |       |
|  RNF006  |       |       |       |       |       |       |       |       |       |       |

# Possíveis features bônus

- **[RB000]** - O sistema deve ser desenvolvido de forma que possa ser executado em aplicativos nativos para Android e iOS.
- **[RB000]** - Como usuário poderei manipular os filtros das tabelas para reordená-las por campo.
- **[RB000]** - Como administrador MASTER poderei gerar os boletos automaticamente de acordo com minha necessidade.


Criado em Abril de 2024 por Daniel Cassemiro Alves 