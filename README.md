# Chatbot Corporativo de RH com RAG

## Sobre o Projeto

Este projeto foi desenvolvido durante uma formação promovida pela Oracle em parceria com a Alura.

O objetivo foi criar um assistente virtual de RH integrado ao Telegram, capaz de responder dúvidas sobre políticas internas da empresa e consultar informações de funcionários armazenadas em banco de dados.

O chatbot foi construído utilizando automação no n8n, Inteligência Artificial Generativa através da Cohere e o conceito de RAG (Retrieval-Augmented Generation), permitindo respostas contextualizadas e alinhadas à base de conhecimento da empresa.

---

## Estrutura do projeto

- chatbot-rh → export do n8n (fluxo principal)
- docs/ → imagens e diagramas
- README.md → explicação do projeto

## Tecnologias

- n8n (automação)
- JSON (workflow de integração)
- Cohere (IA generativa)
- MySQL (banco de dados)
- 
## Problema Resolvido

Empresas frequentemente recebem dúvidas repetitivas relacionadas a:

* Férias
* Banco de horas
* Horários de trabalho
* Políticas internas
* Procedimentos de RH

O projeto teve como objetivo centralizar essas informações em um único canal de atendimento automatizado através do Telegram.

---

## Como Funciona

1. O funcionário envia uma mensagem pelo Telegram.
2. O n8n recebe a solicitação.
3. O agente de IA identifica a intenção da pergunta.
4. Para dúvidas sobre políticas internas, o sistema consulta uma base vetorial utilizando RAG.
5. Para informações pessoais, o sistema consulta o banco de dados MySQL.
6. A resposta é gerada pela IA utilizando apenas informações autorizadas.
7. O resultado é enviado de volta ao usuário no Telegram.

---

## Arquitetura da Solução

Telegram
↓
n8n
↓
Agente de IA (Cohere)
↓
RAG + Vector Store
↓
MySQL
↓
Resposta ao usuário

---

## Tecnologias Utilizadas

* n8n
* Telegram Bot API
* Cohere
* Railway
* MySQL
* Embeddings
* Vector Store
* RAG (Retrieval-Augmented Generation)
* Inteligência Artificial Generativa

---

## Principais Aprendizados

Durante o desenvolvimento deste projeto tive meu primeiro contato com diversos conceitos e ferramentas do ecossistema de IA:

* Construção de fluxos de automação utilizando n8n
* Integração entre aplicações por APIs
* Criação de agentes de IA
* Uso de embeddings para representação semântica de informações
* Implementação de busca vetorial
* Aplicação prática de RAG
* Integração entre IA e banco de dados relacionais
* Desenvolvimento de soluções voltadas para ambientes corporativos

---

## Conceito de RAG Utilizado

O chatbot foi projetado para responder exclusivamente sobre políticas e procedimentos de RH.

Para isso, foi utilizada a abordagem RAG (Retrieval-Augmented Generation), na qual a IA consulta uma base de conhecimento antes de gerar uma resposta.

Dessa forma, as respostas permanecem alinhadas às informações oficiais da empresa, reduzindo alucinações e aumentando a confiabilidade do sistema.

---

## Demonstração

Adicionar imagem do fluxo desenvolvido no n8n.

![Fluxo da solução](docs/fluxo-n8n.png)

---

## Créditos

Projeto desenvolvido durante a formação da Oracle em parceria com a Alura, com foco em Inteligência Artificial, automação de processos e integração de sistemas.
