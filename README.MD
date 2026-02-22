# 🎙️ Voice AI Assistant

Assistente de Voz Inteligente desenvolvido em Python utilizando:

* 🎤 Captura de áudio no Google Colab
* 🧠 Transcrição automática com Whisper
* 🤖 Geração de resposta com OpenAI (fallback Gemini)
* 🔊 Conversão de texto em voz (TTS)

Projeto focado em **integração multimodal de IA (voz + linguagem + síntese)

---

## 🚀 Demonstração do Pipeline

```
Áudio → Whisper → LLM → gTTS → Áudio Resposta
```

Fluxo completo:

1. Usuário clica em **🎙️ Gravar**
2. O navegador captura o áudio
3. O Whisper transcreve a fala
4. A LLM gera resposta contextual
5. O sistema converte texto em voz
6. A resposta é reproduzida automaticamente

---

## 🧠 Tecnologias Utilizadas

* Python 3.10+
* [OpenAI API](https://platform.openai.com/)
* [Google Gemini API](https://aistudio.google.com/)
* Whisper (Speech-to-Text)
* gTTS (Text-to-Speech)
* HTML + JavaScript (Interface no Colab)

---

## 📦 Instalação

No Google Colab:

```python
!pip install git+https://github.com/openai/whisper.git
!pip install openai
!pip install google-generativeai
!pip install gTTS
```

---

## 🔑 Configuração de API Keys

### 🔵 OpenAI (Principal)

1. Crie uma conta em:
   [https://platform.openai.com](https://platform.openai.com)
2. Vá em **API Keys**
3. Clique em **Create API Key**

No Colab:

```
Menu lateral → 🔑 Secrets → Adicione:
OPENAI_API_KEY
```

---

### 🟢 Google Gemini (Fallback)

1. Acesse:
   [https://aistudio.google.com/](https://aistudio.google.com/)
2. Gere sua API Key

No Colab:

```
Menu lateral → 🔑 Secrets → Adicione:
GOOGLE_API_KEY
```

---

## ▶ Como Usar

1. Execute todas as células do notebook
2. Clique no botão:

```
🎙️ Gravar
```

3. Fale por 5 segundos
4. Aguarde a transcrição e resposta
5. O áudio da resposta será reproduzido automaticamente

---

## 🏗️ Arquitetura do Projeto

```
voice-ai-assistant/
│
├── voice_assistant.ipynb
├── README.md
└── requirements.txt
```

---

## 🔒 Segurança

* Nenhuma chave de API é armazenada no código
* Uso de variáveis de ambiente (Secrets do Colab)
* Compatível com renderização no GitHub
* Não utiliza `ipywidgets` (evita erro metadata.widgets)

---

## 🎯 Objetivo do Projeto

Demonstrar:

* Integração com múltiplas APIs
* Tratamento de fallback entre modelos
* Processamento multimodal (voz + texto + voz)
* Boas práticas de segurança


## 👨‍💻 Autor

**Felipe Luna**

Projeto desenvolvido para portfólio e estudo de Inteligência Artificial aplicada.


# ⭐ Se este projeto foi útil, considere dar uma estrela no repositório.
