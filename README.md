# 🎙️ Assistente de Voz Inteligente (Whisper + ChatGPT)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-green.svg)](https://platform.openai.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Este projeto é um assistente virtual integrado desenvolvido durante o laboratório da **DIO**. Ele é capaz de capturar áudio, transcrever, processar uma resposta inteligente via ChatGPT e retornar a resposta sintetizada em áudio.

---

## 🚀 Como funciona?

O pipeline de processamento foi desenhado para seguir um fluxo contínuo de IA:

1.  **Captura (Frontend):** Interface JavaScript no Google Colab captura o áudio do microfone.
2.  **Transcrição (STT):** OpenAI Whisper processa o áudio e converte em texto.
3.  **Processamento (LLM):** ChatGPT (GPT-3.5/4o) analisa a entrada e gera uma resposta contextual.
4.  **Síntese (TTS):** gTTS (Google Text-to-Speech) converte a resposta textual em um arquivo de áudio.

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Função |
| :--- | :--- |
| **Python** | Linguagem principal do pipeline. |
| **OpenAI Whisper** | Transcrição de fala para texto (Speech-to-Text). |
| **OpenAI API** | Inteligência Artificial para processamento de linguagem. |
| **gTTS** | Síntese de voz (Text-to-Speech). |
| **JavaScript** | Integração da API de microfone no navegador. |

---

## ⚙️ Como executar

Como o projeto foi desenvolvido no **Google Colab**, siga estes passos para configurar o ambiente:

1.  **Chave da API:**
    * Obtenha sua `OPENAI_API_KEY` na [plataforma da OpenAI](https://platform.openai.com/).
    * No Google Colab, vá em **"Segredos" (ícone de chave na lateral esquerda)**.
    * Adicione um novo segredo com o nome `OPENAI_API_KEY` e cole o valor da sua chave.
    * Ative a opção "Notebook access" (Acesso ao notebook).

2.  **Execução:**
    * Abra o arquivo `.ipynb` no Google Colab.
    * Conecte-se a um ambiente de execução (GPU é recomendada para o Whisper).
    * Execute as células sequencialmente.

---

## 📦 Estrutura do Repositório

```text
├── Assistente_de_Voz.ipynb  # Notebook principal com o fluxo de IA
├── README.md                # Documentação do projeto
└── requirements.txt         # Dependências do sistema (opcional)
