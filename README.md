<div align="center">
<h1 align="center">🤖 HR Buddy — Assistente Virtual de RH</h1>
</div>

Assistente virtual de Recursos Humanos desenvolvido com **n8n**, **Telegram**, **MySQL**, **Cohere AI** e **Vector Store**, capaz de responder dúvidas de colaboradores, consultar informações de funcionários e fornecer suporte automatizado de RH.

---

## 📌 Sobre

O **HR Buddy** foi desenvolvido para automatizar o atendimento interno de Recursos Humanos da empresa fictícia **ChocolaTech**.

O assistente é capaz de:

* Identificar funcionários por nome completo.
* Consultar informações armazenadas em banco de dados MySQL.
* Responder dúvidas relacionadas a férias e banco de horas.
* Utilizar uma base de conhecimento para responder perguntas gerais de RH.
* Interagir diretamente pelo Telegram.
* Manter contexto das conversas utilizando memória integrada.

> 💡 Projeto desenvolvido como parte das atividades práticas da **Imersão do Programa MCIO & ONE (Oracle Next Education)**, uma iniciativa realizada pela **Oracle**, **Alura** e **Academia MCIO Brasil**, com foco na capacitação e desenvolvimento de talentos na área de tecnologia.

---

## 🛠 Tech Stack

* **n8n** – Plataforma de automação e orquestração de fluxos.
* **Telegram Bot API** – Comunicação com os usuários.
* **MySQL** – Armazenamento dos dados dos funcionários.
* **Cohere AI** – Modelo de linguagem responsável pelas respostas.
* **Simple Memory** – Memória de contexto das conversas.
* **Simple Vector Store** – Base de conhecimento para consultas de RH.
* **Embeddings Cohere** – Vetorização dos documentos da base de conhecimento.

---

## 🚀 Funcionalidades

* 🤖 Atendimento automatizado via Telegram.
* 👤 Identificação de funcionários pelo nome completo.
* 🏖 Consulta de saldo de férias.
* ⏱ Consulta de banco de horas.
* 📚 Respostas baseadas em políticas internas de RH.
* 🧠 Memória de conversação.
* 🔎 Busca semântica em documentos utilizando Vector Store.
* 💬 Integração entre IA generativa e banco de dados.

---

## 📂 Arquitetura do Fluxo

```text
Telegram Trigger
       │
       ▼
   AI Agent
       │
 ┌─────┼─────────┐
 │     │         │
 ▼     ▼         ▼
MySQL Memory Vector Store
 │               │
 └───────┬───────┘
         ▼
Telegram Send Message
```

---

## 🔄 Fluxo de Funcionamento

1. O colaborador envia uma mensagem para o bot no Telegram.
2. O AI Agent identifica a solicitação.
3. Caso necessário, consulta os dados do funcionário no MySQL.
4. Perguntas gerais são respondidas utilizando a base de conhecimento.
5. A resposta é enviada de volta ao usuário pelo Telegram.

---

## 🗄 Banco de Dados

Tabela utilizada:

```sql
funcionarios
```

Exemplo de informações armazenadas:

* Nome completo
* Saldo de férias.
* Banco de horas.
* Identificador do funcionário.

---

## 📱 Exemplo de Uso

### Usuário

```text
Meu nome é Maria Eduarda da Costa Barros Gonçalves.
Quantos dias de férias eu tenho?
```

### HR Buddy

```text
Olá, Maria Eduarda!

Seu saldo atual é de 20 dias de férias disponíveis.
Posso ajudar com mais alguma informação?
```

---

## 🎯 Objetivos de Aprendizagem

Durante o desenvolvimento deste projeto foram praticados:

* Construção de agentes de IA no n8n.
* Integração entre IA e bancos de dados.
* Automação de processos corporativos.
* Desenvolvimento de chatbots para Telegram.
* Uso de memória e contexto em agentes inteligentes.
* Busca semântica utilizando embeddings e Vector Store.
* Engenharia de prompts para agentes de IA.
* Integração entre múltiplas ferramentas e serviços.

---

## ⚠️ Aviso

Este projeto foi desenvolvido para fins educacionais e demonstração de conhecimentos em automação, inteligência artificial e integração de sistemas.

Os dados utilizados são fictícios e não representam informações reais de funcionários.



