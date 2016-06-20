# Ongbook.org - Catálogo de Entidades Sociais e suas Necessidades
Criação social é o futuro da indústria, ainda mais quando se trata da nossa, a de software: bem-vindo à era das multidões! Bem-vindo à era do crowdsourcing!

>Por definição, o <a href="https://pt.wikipedia.org/wiki/Crowdsourcing" target="_blank">crowdsourcing</a> combina os esforços de voluntários identificados ou de trabalhadores em tempo parcial, num ambiente onde cada colaborador, por sua própria iniciativa, adiciona uma pequena parte para gerar um resultado maior.

Nossa documentação está aberta para acompanharem e participarem. Sua evolução será gerenciada através deste repositório (aqui mesmo!). Mais informações sobre o desenvolvimento do projeto estão disponíveis em [Ongbook.org](http://ongbook.org). 

## <a name="topo"></a>Conteúdos

1. [Descrição do projeto](#descricao-do-projeto)
    * [Visão geral](#visao-geral)
    * [Objetivos](#objetivos)
    * [Mini Mundo](#projeto-de-mini-mundo)
1. [Documento de requisitos](documento-de-requisitos)

* Documentação do back-end - **<a href="https://github.com/Ongbook/api-nodejs" target="_blank">api-nodejs</a>**
* Documentação do front-end - **<a href="https://github.com/Ongbook/consummer-angularjs" target="_blank">consummer-angularjs</a>**
* Apresentação da iniciativa na **<a href="https://github.com/Ongbook/documentacao/wiki" target="_blank">Wiki</a>** (Associação, equipe, entre outros)

## <a name="descricao-do-projeto"></a> Descrição do projeto
Como o nome já diz, _Ongbook_, Livro de ONGs. Um catálogo digital de Entidades filantrópicas. Essas Entidades poderão cadastrar suas necessidades, que por ventura venham surgir: bens materiais :jeans:, mão de obra (trabalho voluntariado :muscle:) e de recursos financeiros (doação :moneybag:). Necessidades serão objetos da aplicação, as quais poderão ser listadas por diferentes filtros (localização pela região, área de atuação, proximidades, entre outros).

A aplicação é especializada em levar essas informações (_necessidades_) ao seu público-alvo (_usuários, pessoas físicas com perfis solidários_), com o objetivo de supri-las. Unindo solidários com necessitados.

### <a name="visao-geral"></a>Visão geral

Existe uma carência quando se trata de pessoas com perfil solidário, em manter-se atualizadas e em constante interação com causas e necessidades presentes no dia a dia de Entidades que trabalham para suprir problemas sociais em geral. Também vislumbramos a possibilidade de ajudar essas instituições do terceiro setor, oferecendo uma plataforma online.

### Objetivos

#### Do resultado
- Evidenciar atividades de Entidades Sociais, cadastrando e listando suas necessidades;
- Suprí-las através da interação social;
- Promover voluntariado e incentivar solidariedade;
- Possiblitando que mais pessoas sejam amparadas.

#### Do processo
- Produzir software com qualidade, junto com a comunidade;
- Implantar metodologias ágeis nos processos e fazer o simples e necessário - **<a href="http://gettingreal.37signals.com/GR_por.php" target="_blank">Getting Real</a>**;
- Gerenciar ciclo de vida da aplicação, da concepção dos requisitos ao deploy;
- Entregar valor (funcionalidades) em cilcos, testando as hipóteses junto ao publico usuário (De um lado, os coordenadores de Entidades Sociais, no outro, usuários solidários).
- O mais importante é uma comunicação clara, rica e colaborativa entre os integrantes da equipe, stakeholders, comunidade e usuários. Seguindo os princípios do [Manifesto Ágil](http://www.agilemanifesto.org/iso/ptbr/): *"Os processos ágeis promovem desenvolvimento sustentável"*.

**[⬆ volte ao topo](#topo)**

#### Projeto de Mini Mundo
[DESCRIÇÃO]

**[⬆ volte ao topo](#topo)**

## Requisitos
### Não funcionais
Requisitos que não correspondem de fato a uma funcionalidade da aplicação. Tais requisitos foram divididos em três tipos:
#### De produto
ID | Descrição
------------ | -------------
RNF01 | Deve ser desenvolvido no modelo arquitetural RESTful¹. Separando back-end (API oferecendo recursos via JSON) e front-end, consumindo esses recursos. Que também serão expostos para terceiros
RNF02 | Deve ser implementado com Stack MEAN (MongoDB, Express js, Angular js, Node js)
RNF03 | Hospedado em ambiente Nginx em instancia Linux
##### Usabilidade
ID | Descrição
------------ | -------------
RNF04 | Permitir ao usuário facilidades de uso, com uma interface gráfica intuitiva, garantindo que todas as funcionalidades estejam facilmente acessíveis. E evolua dinamicamente conforme a experiência do usuário (UX). Em browsers, smartphones e smart TVs
##### Segurança
ID | Descrição
------------ | -------------
RNF05 | Configuração de HTTPS, para manter um tráfego encriptado com SSL/TLS
RNF06 | Implementar autenticação OAuth2 para requisições
#### De processo
ID | Descrição
------------ | -------------
RNF07 | Código fonte versionado com Git, exposto em repositórios no Github
RFN08 | Uso de TDD - Desenvolvimento Dirigido a Testes, automatizados. E implementação de ferramentas de integração contínua
##### Documentação
ID | Descrição
------------ | -------------
RFN09 | Devem ser elaborados artefatos e documentos necessários para melhor compreensão dos requisitos descritos. serão elaborados antes do ciclo de desenvolvimento e devem estar abertos a participação pública* na internet
RFN10 | A documentação dos requisitos deve acompanhar os ciclos de desenvolvimento de software (Sprints). Para servir de apoio aos integrantes da equipe, stakeholders e comunidade
#### Externos
##### Econômicos
ID | Descrição
------------ | -------------
RFN11 | A aplicação não deve exigir muito dos recursos (processamento e memória) dos diversos dispositivos nos quais esteja sendo executado. (Browsers PC e mobiles, Smart TVs, app nativos iOS, Android e Win mobile)
##### Legais
ID | Descrição
------------ | -------------
RFN12 | Antes do cadastro na aplicação os usuários deverão ter disponível o **Termo de cadastro de Entidades Sociais** e **Política de Privacidade de Usuários**, a fim de garantir a responsabilidade dos mesmos com as ações realizadas na aplicação

### Funcionais
Os requisitos funcionais descrevem as ações do sistema, isto é, as funções necessárias para alcançar os objetivos do sistema.
#### 1º Sprint
ID | Nome | Prioridade
------------ | ------------- | -------------
RF-1 | Cadastrar Entidade Social | Essencial
RF-2 | Atualizar dados do perfil da Entidade Social | Essencial
RF-3 | Desabilitar, nunca excluir Entidade Social | Essencial
RF-4 | Listar Entidades Sociais por filtros | Essencial
RF-5 | Visualizar perfil da Entidade Social na íntegra | Essencial
**[⬆ volte ao topo](#topo)**
