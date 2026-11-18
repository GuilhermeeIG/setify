<h1 align="center"> Setify</h1>
<p align="center"><b>Plataforma de produção de vídeos curtos com IA, controle de afiliados e pesquisa de mercado avançada</b></p>

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white" /> <img src="https://img.shields.io/badge/FFmpeg-007808?style=for-the-badge&logo=ffmpeg&logoColor=white" /> <img src="https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white" /> <img src="https://img.shields.io/badge/Chrome%20Extension-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white" />
</p>

>  O código-fonte deste projeto é **privado**. Este repositório é uma vitrine com a visão geral, a arquitetura e a stack. Quer saber mais? Fale comigo pelo [LinkedIn](https://www.linkedin.com/in/luiz-guilherme-dos-santos-820a792a4/).

##  O que é

Uma plataforma que automatiza a produção de vídeos curtos (shorts) em escala. Ela é formada por quatro peças que trabalham juntas:

| Peça | Função |
|---|---|
|  **Workspace** | Organiza produtos, roteiros e lotes de vídeos |
|  **Maestro** | Orquestrador desktop: leva cada vídeo pela esteira (geração → download → edição → entrega) com fila em disco e retomada |
|  **Extensão** | Extensão de navegador que automatiza a geração de clipes com IA generativa de vídeo em massa |
|  **Shortify** | Editor desktop que monta o vídeo final sozinho |

##  Shortify: o editor

-  **Transcrição offline** com faster-whisper/CTranslate2, sem API paga e sem GPU obrigatória
-  **Cortes pela fala**: remove pausas e respeita o movimento do avatar
-  **Legendas gravadas no vídeo**, com destaque sincronizado palavra a palavra
-  **Render com FFmpeg** e QA automático do resultado
-  **Processamento em lote** com checkpoints e retomada segura
-  **Timeline de revisão** com prévia de áudio e vídeo antes de exportar
-  **Instaladores para Windows e macOS** (Apple Silicon e Intel) com PyInstaller

##  Stack

- **Desktop:** Python · CustomTkinter · faster-whisper · CTranslate2 · ONNX Runtime · PyAV · NumPy · Pydantic · FFmpeg
- **Extensão:** JavaScript · Chrome Extensions API (Manifest V3)
- **Qualidade:** pytest · ruff · black · GitHub Actions
