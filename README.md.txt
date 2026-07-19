# Sistema de Análise Automática de Dados Técnicos com IA

## 📌 Descrição do Projeto

Este projeto tem como objetivo automatizar a análise de informações técnicas, reduzindo o trabalho manual de interpretação de documentos e desenhos técnicos.

A solução utiliza Inteligência Artificial para receber dados técnicos, analisar as informações enviadas e gerar uma resposta estruturada com os materiais identificados, facilitando a conferência e tomada de decisão da equipe.

---

# 🎯 Problema Identificado

Atualmente, a análise de documentos técnicos é realizada manualmente, demandando tempo da equipe e aumentando a possibilidade de erros na identificação de materiais necessários.

O processo manual dificulta:

* Conferência rápida das informações;
* Organização dos dados;
* Identificação de possíveis faltas de materiais;
* Padronização das análises.

---

# 💡 Solução Desenvolvida

Foi criada uma automação utilizando:

* **Lovable** → Interface para entrada dos dados;
* **Make.com** → Orquestração e automação do processo;
* **Google Gemini AI** → Análise inteligente das informações técnicas;
* **Google Sheets** → Armazenamento e organização dos resultados.

A aplicação recebe os dados enviados pelo usuário, encaminha para a IA realizar a análise e registra automaticamente o resultado em uma planilha.

---

# 🔄 Fluxo da Automação

## 1. Entrada de dados

O usuário preenche um formulário contendo informações como:

* Nome;
* Empresa;
* E-mail;
* Telefone;
* Peça/material;
* Código;
* Descrição técnica;
* Prioridade;
* Observações;
* Arquivo técnico (quando disponível).

---

## 2. Webhook Make.com

O formulário envia os dados para um Webhook do Make.

Responsável por:

* Receber as informações;
* Iniciar o cenário de automação;
* Encaminhar os dados para processamento.

---

## 3. Análise com Google Gemini AI

O Gemini recebe os dados técnicos e realiza uma análise automática.

A IA é utilizada para:

* Interpretar informações técnicas;
* Organizar os dados;
* Identificar materiais;
* Classificar prioridade;
* Gerar uma resposta estruturada.

---

## 4. Registro no Google Sheets

Após a análise, o resultado é salvo automaticamente em uma planilha.

A planilha funciona como banco de dados contendo:

* Dados do solicitante;
* Informações técnicas;
* Resultado da análise da IA;
* Observações.

---

# 🏗️ Arquitetura da Solução

```
Usuário
   |
   ↓
Lovable (Formulário)
   |
   ↓
Webhook Make.com
   |
   ↓
Google Gemini AI
   |
   ↓
Google Sheets
   |
   ↓
Resultado da análise
```

---

# 🛠️ Tecnologias Utilizadas

| Tecnologia       | Função                     |
| ---------------- | -------------------------- |
| Lovable          | Criação da interface web   |
| Make.com         | Automação do fluxo         |
| Google Gemini AI | Processamento inteligente  |
| Google Sheets    | Armazenamento dos dados    |
| Webhooks         | Comunicação entre sistemas |

---

# 📋 Campos Processados

Os principais campos enviados são:

* Nome
* Empresa
* E-mail
* Telefone
* Peça
* Código
* Descrição
* Prioridade
* Observações
* Arquivo técnico

---

# 🚀 Como Executar o Projeto

1. Acessar a aplicação criada no Lovable.
2. Preencher o formulário com os dados técnicos.
3. Enviar a solicitação.
4. O Make receberá os dados automaticamente.
5. O Gemini realizará a análise.
6. O resultado será registrado no Google Sheets.

---

# ✅ Benefícios da Solução

* Redução do trabalho manual;
* Maior velocidade na análise;
* Organização automática das informações;
* Uso de Inteligência Artificial no processo;
* Histórico centralizado dos dados;
* Apoio à tomada de decisão.

---

# 📌 Possíveis Melhorias Futuras

* Leitura automática de arquivos PDF técnicos;
* Comparação entre desenho técnico e lista de materiais;
* Envio de notificações para equipes responsáveis;
* Dashboard de acompanhamento;
* Integração com sistemas corporativos.

---

# 👩‍💻 Desenvolvido por

Greice Lima Rocha

Projeto desenvolvido como solução de automação utilizando ferramentas Low-Code e Inteligência Artificial.
