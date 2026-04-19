🎙️ Assistente de Voz Inteligente (Whisper + ChatGPT)
Este projeto é um assistente virtual integrado desenvolvido durante o laboratório da DIO. Ele é capaz de capturar áudio, transcrever, processar uma resposta inteligente via ChatGPT e retornar a resposta sintetizada em áudio.

🚀 Como funciona?
O pipeline de processamento foi desenhado para seguir um fluxo contínuo de IA:

Captura (Frontend): Interface JavaScript no Google Colab captura o áudio do microfone.

Transcrição (STT): OpenAI Whisper processa o áudio e converte em texto.

Processamento (LLM): ChatGPT (GPT-3.5/4o) analisa a entrada e gera uma resposta contextual.

Síntese (TTS): gTTS (Google Text-to-Speech) converte a resposta textual em um arquivo de áudio.

🛠️ Tecnologias Utilizadas
TecnologiaFunçãoPythonLinguagem principal do pipeline.OpenAI WhisperTranscrição de fala para texto (Speech-to-Text).OpenAI APIInteligência Artificial para processamento de linguagem.gTTSSíntese de voz (Text-to-Speech).JavaScriptIntegração da API de microfone no navegador.

⚙️ Como executar
Como o projeto foi desenvolvido no Google Colab, siga estes passos para configurar o ambiente:

Chave da API:

Obtenha sua OPENAI_API_KEY na plataforma da OpenAI.

No Google Colab, vá em "Segredos" (ícone de chave na lateral).

Adicione um novo segredo com o nome OPENAI_API_KEY e cole o valor da sua chave.

Ative a opção "Notebook access" (Acesso ao notebook).

Execução:

Abra o arquivo .ipynb no Google Colab.

Conecte-se a um ambiente de execução (GPU é recomendada para o Whisper).

Execute as células sequencialmente.

📦 Estrutura do Repositório
├── Assistente_de_Voz.ipynb  # Notebook principal com o fluxo de IA
├── README.md                # Documentação do projeto
└── requirements.txt         # Dependências do sistema (opcional)

