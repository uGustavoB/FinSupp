# Visão do produto

## Finsupp \- Sistema de gestão financeira

## Sumário


- [Introdução](#introdução)
  - [Propósito](#propósito)
  - [Definições](#definições)

  - [Escopo do produto](#escopo-do-produto)
- [Posicionamento](#posicionamento)
  - [Oportunidade de negócio](#oportunidade-de-negócio)
  - [Descrição dos benefícios para os clientes e dos problemas resolvidos](#descrição-dos-benefícios-para-os-clientes-e-dos-problemas-resolvidos)
- [Descrição dos stakeholders e dos usuários](#descrição-dos-stakeholders-e-dos-usuários)
  - [Stakeholders](#stakeholders)
  - [Usuários e atores](#usuários-e-atores)
- [Descrição do ambiente de uso](#descrição-do-ambiente-de-uso)
  - [Ambiente de uso](#ambiente-de-uso)
  - [Necessidades principais quanto ao ambiente](#necessidades-principais-quanto-ao-ambiente)
- [Custo e Venda](#custo-e-venda)
- [Licenciamento e Instalação](#licenciamento-e-instalação)
- [Características e Funcionalidades de Alto Nível](#características-e-funcionalidades-de-alto-nível)
- [Restrições](#restrições)


# Introdução 

O Documento de Visão do Produto (DVP) é um documento que descreve o produto de software que será desenvolvido. Ele descreve o problema que será resolvido, as principais necessidades dos stakeholders, as principais funcionalidades do sistema, as restrições do projeto, etc.

## Propósito

O propósito do FinSupp é fornecer uma plataforma acessível e intuitiva para o gerenciamento financeiro, ajudando os usuários a tomarem decisões informadas sobre seus gastos, economias e investimentos.

Por recursos como categorização de despesas, geração de relatórios e alertas personalizados, o FinSupp visa capacitar os usuários a alcançarem seus objetivos financeiros e a manterem um controle eficaz de suas finanças pessoais.

## Definições

| Termo | Definição |
| :---- | :---- |
| FinSupp | Nome da plataforma digital de gestão financeira pessoal. |
| Cliente | Pessoa física ou jurídica que adquire ou utiliza a plataforma FinSupp. |
| Usuário | Pessoa que utiliza ativamente o sistema para controle financeiro. |

## Escopo do produto

O FinSupp é um sistema de gestão financeira que permite aos usuários registrar, categorizar e acompanhar suas finanças pessoais proporcionando uma experiência integrada e facilitando o acesso às informações financeiras em qualquer lugar e a qualquer momento.

O sistema é projetado para atender tanto usuários individuais quanto pequenas empresas, oferecendo recursos específicos para cada perfil de usuário.

# Posicionamento

## Oportunidade de negócio

O FinSupp apresenta várias oportunidades de negócios, tais como:

1. Mercado de Finanças Pessoais em Expansão  
   O mercado de aplicativos e plataformas de finanças pessoais cresce continuamente, impulsionado pela digitalização bancária, aumento do uso de cartões e necessidade crescente de controle financeiro. O FinSupp pode entrar nesse mercado como uma solução acessível e personalizável para usuários que buscam mais controle sobre seus gastos e receitas.

2. Oferta como SaaS (Software as a Service)  
   Transformar o FinSupp em uma plataforma SaaS permitiria monetizar por meio de planos mensais ou anuais, oferecendo diferentes níveis de funcionalidades (ex: plano gratuito com funcionalidades básicas e planos pagos com acesso a relatórios avançados, controle familiar, entre outros).

3. Parcerias com Educadores Financeiros e Influenciadores  
   O produto pode ser oferecido como ferramenta complementar para educadores financeiros, coaches ou influenciadores que desejam recomendar soluções práticas a seus seguidores. Isso abre portas para parcerias, licenciamento e co-branding.

4. Versão Corporativa ou Multiusuário  
   Expandir o escopo para micro e pequenas empresas que precisam de um controle básico de finanças pode abrir um novo segmento de mercado. Isso incluiria controle de fluxo de caixa, separação de contas por departamentos, e múltiplos usuários com permissões distintas.

5. Integrações com Bancos e Fintechs  
   Ao adicionar integrações futuras com APIs de bancos e fintechs, o FinSupp poderia se tornar um hub financeiro centralizado, atraente para parcerias com instituições financeiras ou carteiras digitais que queiram mais valor aos seus clientes.

6. White-label para Profissionais ou Consultores  
   O sistema pode ser licenciado como uma solução white-label para profissionais da área financeira que desejem oferecer um aplicativo de controle financeiro com sua própria marca.

7. Gamificação para Engajamento  
   A inclusão de elementos de gamificação (metas, desafios de economia, recompensas) pode aumentar o engajamento dos usuários e criar oportunidades para parcerias com empresas de educação financeira ou plataformas de fidelidade.

## Descrição dos benefícios para os clientes e dos problemas resolvidos {#descrição-dos-benefícios-para-os-clientes-e-dos-problemas-resolvidos}

| Benefícios | Problemas Resolvidos | Afetados |
| :---- | :---- | :---- |
| Organização financeira centralizada | Dificuldade em controlar contas, cartões, despesas e receitas em um só lugar | Usuários com múltiplas contas e fontes de gasto |
| Maior consciência financeira | Falta de visibilidade clara sobre onde e como o dinheiro está sendo gastos | Pessoas que perdem o controle do orçamento mensal |
| Planejamento de despesas | Incerteza quanto a cobranças recorrentes e despesas futuras | Usuários com assinaturas ou faturas em diversas contas |
| Facilidade no controle de gastos | Complexidade para registrar e acompanhar transações diárias | Usuários sem conhecimento técnico em finanças e sistemas |
| Alertas personalizados | Falta de notificação ao exceder teto de gastos | Clientes que perdem controle de seus gastos |

## Descrição dos stakeholders e dos usuários

Esta seção descreve os principais stakeholders e usuários do FinSupp, suas necessidades e como o sistema atende a essas demandas.

### Stakeholders

| Stakeholder | Descrição | Papel |
| :---- | :---- | :---- |
| Equipe de Desenvolvimento | Responsável pelo desenvolvimento e manutenção do sistema | Desenvolver e manter a aplicação |
| Equipe de Marketing | Responsável pela promoção e divulgação do FinSupp, junto às Entidades do ramo financeiro | Profissionais responsáveis pela divulgação do sistema |
| Consultores/Educadores Financeiros | Profissionais que podem utilizar ou recomendar o sistema como ferramenta para seus clientes | Possível parceiro comercial para divulgação do produto, e atraindo clientes |
| Entidades do ramo financeiro  | Entidades que do ramo financeiro que não possuem um sistema de controle financeiro para disponibilizar para seus clientes  | Fornecer o produto para seus clientes, agindo como distribuidor do produto |
| Departamento de análise econômica | Profissionais oriundos das entidades financeiras, que fornecem suporte em relação a decisões financeiras  | Fornecer suporte na implementação de metas financeiras automatizadas e nos relatórios e análises gerados |
| Gerente de Projeto | Profissional responsável por gerenciar o projeto e garantir que o sistema seja entregue dentro do prazo e orçamento definidos | Gerenciar equipes e andamento do projeto |
| Usuários | Pessoas que buscam uma solução para organizar suas finanças de forma centralizada | Usuário do sistema |

### Usuários e atores

| Usuário | Descrição | Responsabilidades | Stakeholders |
| :---- | :---- | :---- | :---- |
| Usuário | Pessoa que utiliza o sistema para gerenciar suas finanças pessoais. | Registrar despesas, receitas e acompanhar o saldo. | Equipe de Desenvolvimento, Equipe de Marketing, Gerente de projeto |
| Atendente de suporte | Profissional responsável por atender os usuários, que apresentem problemas ao utilizar o sistema | Atender e sanar as dúvidas em relação a utilização da plataforma e funcionalidades específicas  | Usuários, Equipe de desenvolvimento, Gerente de Projeto, Departamento de atendimento ao cliente |
| Administrador | Pessoa responsável por gerenciar o sistema e os usuários. | Configurar o sistema, gerenciar usuários e permissões e supervisionar o uso da aplicação | Equipe de Desenvolvimento, Gerente de projeto |
| Entidades financeiras (Open Finance) | Entidades que podem disponibilizar os dados dos seus clientes que adotarem a plataforma FinSupp | Disponibilizar dados dos clientes interessados através de Open Finance | Usuários, Equipe de desenvolvimento, Gerente de Projeto, Entidades financeiras |

# **Descrição do ambiente de uso**

## **Ambiente de uso**

Abaixo estão apresentados os diferentes contextos em que o sistema pode ser utilizado:

1. **Ambiente do Usuário**: este é o espaço destinado ao uso dos usuários para o controle de suas finanças pessoais. O acesso pode ser feito por meio de dispositivos móveis, como smartphones e tablets, ou por navegadores web em computadores. Os navegadores compatíveis incluem Google Chrome, Mozilla Firefox e Microsoft Edge. O aplicativo estará disponível para os sistemas Android e iOS. Esse ambiente é acessado via internet e exige autenticação com login e senha.

2. **Ambiente Administrativo**: utilizado pelos administradores para a gestão e manutenção do sistema. O acesso é realizado por meio de navegadores web em computadores, permitindo o uso de funcionalidades como administração de usuários, realização de backups e aplicação de atualizações no sistema.

3. **Ambiente de Testes**: este ambiente é voltado para a validação de novas funcionalidades e correções antes da liberação oficial aos usuários. O acesso é feito através de navegadores web em computadores e exige credenciais específicas para esse ambiente.

## **Necessidades principais quanto ao ambiente**

A seguir, é apresentada uma tabela que descreve as necessidades dos clientes com relação à qualidade, desempenho, segurança e usabilidade do sistema FinSupp, juntamente com sua prioridade, interesse, solução atual e soluções propostas:

| Necessidade | Prioridade | Interesse | Solução atual | Soluções propostas |
| :---- | :---- | :---- | :---- | :---- |
| **Qualidade:** o sistema deve garantir alta disponibilidade, confiabilidade, precisão, portabilidade e robustez, estando sempre disponível e livre de erros essenciais. | Alta | Os usuários esperam que o sistema funcione continuamente sem interrupções, permitindo acesso às suas informações financeiras a qualquer momento, com dados precisos e confiáveis para tomada de decisões. | Controle manual das finanças através de planilhas ou aplicativos básicos, sujeitos a falhas e indisponibilidade. | Implementar arquitetura em nuvem com alta disponibilidade, testes automatizados rigorosos, validação de dados em tempo real, design responsivo para múltiplas plataformas e tratamento robusto de exceções para garantir estabilidade do sistema. |
| **Desempenho:** o sistema deve oferecer tempo de resposta rápido, capacidade de escalabilidade e resposta consistente, mesmo com o crescimento da base de usuários. | Alta | Os usuários necessitam de acesso instantâneo às suas informações financeiras, com performance consistente independentemente do número de transações ou usuários simultâneos no sistema. | Aplicativos lentos ou que apresentam degradação de performance com o aumento de dados, causando frustração e perda de produtividade. | Otimizar consultas de banco de dados, implementar cache inteligente, utilizar CDN para recursos estáticos, arquitetura de microserviços escalável, balanceamento de carga automático e monitoramento contínuo de performance com alertas proativos. |
| **Segurança:** o sistema deve garantir proteção contra acessos indevidos, confidencialidade dos dados, proteção contra ataques, gerenciamento seguro de senhas e auditoria completa com monitoramento através de logs. | Alta | Os usuários precisam ter total confiança na proteção de seus dados financeiros sensíveis, com garantia de que apenas pessoas autorizadas tenham acesso às informações e que todas as atividades sejam monitoradas. | Controles básicos de segurança em aplicativos existentes, muitas vezes inadequados para proteção de dados financeiros sensíveis. | Implementar autenticação multifator (2FA), criptografia end-to-end para dados sensíveis, certificados SSL/TLS, política de senhas robusta, monitoramento de segurança 24/7, logs de auditoria detalhados e conformidade com LGPD. |
| **Usabilidade:** o sistema deve proporcionar fácil personalização (temas, cores), interface clara e intuitiva, mensagens de erro claras e feedback rápido ao usuário. | Moderada | Os usuários esperam uma experiência agradável e eficiente, com interface que se adapte às suas preferências pessoais e que seja fácil de navegar, mesmo para pessoas com pouco conhecimento técnico. | Interfaces complexas e pouco intuitivas em soluções existentes, com dificuldade de personalização e mensagens de erro técnicas confusas. | Desenvolver interface responsiva com design system moderno, sistema de temas personalizáveis (claro/escuro), mensagens de erro em linguagem simples com sugestões de solução, tooltips e ajuda contextual, testes de usabilidade com usuários reais e implementação de feedback visual imediato para todas as ações do usuário. |

**Visão geral do produto**

**Visão Geral**

O FinSupp é um sistema de controle financeiro pessoal que permite aos usuários organizarem, monitorarem e gerenciarem suas finanças de maneira simples, prática e centralizada. Por meio da plataforma, os usuários podem registrar receitas e despesas, categorizar transações, acompanhar metas financeiras.

Como o FinSupp é um software baseado na web, sua estrutura operacional é sustentada por uma infraestrutura de TI. Isso inclui servidores, banco de dados e dispositivos de rede, como switches e roteadores, necessários para garantir a estabilidade e o acesso seguro à plataforma.

O sistema pode ser acessado por meio de navegadores web em dispositivos como computadores, laptops, tablets e smartphones, desde que estejam conectados à internet. Essa característica permite que os usuários acompanhem e gerenciem suas finanças a qualquer hora e de qualquer lugar. Desse modo, o sistema também oferece acesso a aparelhos mobiles de maneira offline pelo aplicativo, porém os dados só são enviados e atualizados quando conectados a internet.

A interação entre os dispositivos e o servidor do FinSupp ocorre por meio de conexões de rede, utilizando protocolos como o HTTP para a comunicação entre cliente e servidor. Isso possibilita que os dados sejam atualizados em tempo real, promovendo uma experiência fluida e responsiva para o usuário.

Além disso, o FinSupp pode ser integrado com outros sistemas e serviços financeiros por meio de APIs, o que permite, por exemplo, a sincronização automática de dados bancários, parcerias com fintechs ou o fornecimento de dados para consultorias financeiras. Essas integrações ampliam a funcionalidade da plataforma e fortalecem sua proposta como um hub financeiro digital completo.

Uma estrutura operacional do produto é apresentada na Figura 1.


![https://github.com/uGustavoB/FinSupp/figura1.png][image1]
**Figura 1** - Arquitetura ambiental do sistema FinSupp



### **Custo e Venda**

A decisão sobre a viabilidade econômica do requisito de planejamento financeiro do sistema FinSupp é aplicável ao departamento comercial, ao gerente de projetos e a potenciais clientes interessados na aquisição e implantação da solução.

### **Licenciamento e Instalação**

O sistema FinSupp será disponibilizado mediante a concessão de uma licença de uso, emitida pela empresa desenvolvedora. A licença permitirá ao cliente instalar e utilizar o software em servidores próprios ou em uma nuvem pública, desde que sejam respeitadas as condições mínimas de infraestrutura descritas no documento oficial de instalação.

A instalação poderá ser realizada de forma autônoma pelo cliente ou pela equipe técnica da empresa desenvolvedora, caso o cliente opte pela contratação do serviço adicional de instalação e configuração.

Durante o processo de instalação, serão feitas as devidas configurações de ambiente, criação do banco de dados e ajustes de rede necessários para o correto funcionamento do sistema. Será fornecido um guia detalhado de instalação, além de suporte técnico especializado, se necessário.

Após a instalação, o cliente receberá credenciais de acesso para começar a utilizar todas as funcionalidades do sistema FinSupp.

### **Características e Funcionalidades de Alto Nível**

Esta seção apresenta os principais requisitos de alto nível do sistema FinSupp, essenciais para gerar valor aos seus usuários:

* O sistema deve permitir o cadastro de clientes, contas e categorias de gastos/receitas, com dados detalhados.

* O sistema deve enviar alertas financeiros automáticos via e-mail ou aplicativo, como lembretes de vencimento de contas ou metas ultrapassadas.

* O sistema deve permitir visualização e análise de relatórios financeiros, com filtros por período, categoria e tipo de despesa.

* O sistema deve contar com gráficos interativos para facilitar o entendimento do comportamento financeiro do usuário.

* O sistema deve garantir a segurança das informações financeiras, com autenticação forte, criptografia de dados e controle de permissões.

* O sistema deve oferecer uma interface intuitiva, acessível para diversos perfis de usuários, incluindo iniciantes em gestão financeira.

* O sistema deve ter bom desempenho e alta disponibilidade, com tempo de resposta rápido e funcionamento contínuo.

* O sistema deve ser escalável, para comportar o crescimento de usuários e dados sem comprometer a performance.

* O sistema será desenvolvido conforme boas práticas de engenharia de software e normas técnicas da indústria.

* O código-fonte do sistema será documentado e mantido sob versionamento, possibilitando auditorias e manutenção futuras.

### 

### **Restrições** 

Algumas restrições a serem observadas no desenvolvimento e implantação do sistema FinSupp:

* **Orçamento:** O projeto deve ser executado dentro do limite orçamentário aprovado previamente.

* **Tempo:** O sistema deve ser entregue em até 12 meses, com entregas quinzenais de MVP (Produto Mínimo Viável).

* **Hardware:** O sistema deve ser compatível com a infraestrutura moderna atual, não suportando hardware obsoleto.

* **Segurança e privacidade:** Deve estar em conformidade com a LGPD (Lei Geral de Proteção de Dados).

* **Usabilidade:** A interface deve ser acessível a usuários com deficiência visual ou motora, em conformidade com as diretrizes de acessibilidade.

* **Interoperabilidade:** O sistema deve ser capaz de integrar-se com outras plataformas e sistemas contábeis/financeiros via APIs.

* **Desempenho:** Deve garantir alta performance, com escalabilidade e disponibilidade adequadas ao volume esperado.

* **Geografia e Idioma:** O sistema deve considerar fusos horários e estar disponível no idioma portuguêsl.