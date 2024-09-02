# Deploying your own LLM

You need a model and an interface of your choice.

RAG - Retreival-Augmented Generation.

## Curated lists of UIs
* [JShollaj's Awesome LLM WebUIs](https://github.com/JShollaj/Awesome-LLM-Web-UI)

## LLM + WebUI

* [Oobabooga Text Generation UI](https://github.com/oobabooga/text-generation-webui) now supports one-click install
* [SillyTavern](https://docs.sillytavern.app/) for [Windows](https://docs.sillytavern.app/installation/windows/), [Linux & Mac](https://docs.sillytavern.app/installation/linuxmacos/). There is also a [Simple Launcher](https://sillytavernai.com/st-simplelauncher/) available.
* [ChatUI](https://github.com/huggingface/chat-ui) - UI with web search.
* [lollms-webui](https://github.com/ParisNeo/lollms-webui/) - Has PDF, stable diffusion and web search integration
* https://github.com/h2oai/h2ogpt - Has PDF, Web search, best for files ingestion (supports many file formats)
* https://github.com/NimbleBoxAI/ChainFury - Has great UI and web search (experimental)
* https://github.com/nomic-ai/gpt4all - Basic UI that replicated ChatGPT
* https://github.com/imartinez/privateGPT - Basic UI that replicated ChatGPT with PDF integration
* [Telemate](https://github.com/vegu-ai/talemate) - Focus on strong world, narration, and state tracking

With citations and RAG:
* [Perplexica](https://github.com/ItzCrazyKns/Perplexica) - UI with a search engine, that can use local LLMs, just like Perplexity, but local
* [OpenPerplex Backend OS](https://github.com/YassKhazzan/openperplex_backend_os) - 

More from the comments (Haven't tested myself) :
* https://github.com/LostRuins/koboldcpp - Easy to install and simple interface
* LM Studio - Clean UI, focuses on GGUF format
* https://github.com/lobehub/lobe-chat - Nice rich UI with the ability to load extensions for web search, TTS and more
* https://github.com/ollama-webui/ollama-webui - ChatGPT like UI with easy way to download models
* https://github.com/turboderp/exui - very fast and vram efficient
* https://github.com/PromtEngineer/localGPT - Focuses on PDF files
* https://github.com/shinomakoi/AI-Messenger - Supports EXLv2 and LLava
* [big-AGI](https://github.com/enricoros/big-AGI)
* Documentation - Vercel AI SDK - NodeJS/Reactive
* FreeChat - some love to MacOS
* Sanctum - another MacOS GUI

## Adding LLM files
In Ooobabooga you just download models from the interface or put them into the "models" directory, and then load them.

## Adding speech synthesis (Text-To-Speech)
* In [SillyTavern](https://docs.sillytavern.app/extras/extensions/tts/)

## Adding speech recognition (Speech-To-Text)
* In [SillyTavern](https://docs.sillytavern.app/extras/extensions/speech-recognition/)
