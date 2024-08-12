# ARCANE Manual: Advaced Refined Customised Artificial Neural Entities

*by Starlight Robotics*

ARCANE Manual is a curated repository of AI Role-playing LLMs, chatbots, services, apps, interfaces, offline tools, and hardware tips. This manual provides insight for where to start, and reference links for seasoned developers.

Local essentials:
* [Hardware](hardware.md) is needed to run LLMs locally
* [LLM Deployment and User Interface](deployment-and-ui.md) of your own LLM
* [Chatbot Frameworks](chatbot-frameworks.md) for public presence
* [Specialist models](specialist-models.md) - medicine, finance, law
* [⭐ Big Code Models Leaderboard](https://huggingface.co/spaces/bigcode/bigcode-models-leaderboard) - coding models

Online:
* [Online services and apps](online-services.md) for Role-play are available, paid and free
* Image generation models can be found on [CivitAI](https://civitai.com/)

Advancements:
* [Challenges and Limits](challenges.md) that we face and need to be solved
* [Awesome LLM-Powered Agent](https://github.com/hyp1231/awesome-llm-powered-agent#human-interaction-simulation) - source for papers, specifically [Human Interaction Simulation](Awesome LLM-Powered Agent)

Help:
* ARCANE Manual has a [FAQ](faq.md) section
* To suggest updates and edits or just introduce yourself, you can contact me on [Reddit](https://www.reddit.com/r/starlightrobotics/) or [Discord](https://discord.gg/zarD7dweKz)

## LLMs / Models

**The 2023 LLMs that made some noise**

* [PygmalionAI](https://github.com/PygmalionAI) - 
All models: [HuggingFace](https://huggingface.co/PygmalionAI), Most popular of which as of October 2023 is [Mythalion 13B](https://huggingface.co/PygmalionAI/mythalion-13b) - A merge of Pygmalion-2 13B and MythoMax 13B

* [MythoMax 13B](https://huggingface.co/Gryphe/MythoMax-L2-13b) - by Gryphe. Uncensored.

* Mistral 7B and [SynthIA](https://huggingface.co/TheBloke/Synthia-7B-v1.3-GGUF) - Uncensored, trained on Mistral

* [CalliopeDS](https://huggingface.co/Doctor-Shotgun/CalliopeDS-L2-13B) - This is a Llama 2-based model consisting of a merge of several models using a weight-adjusted TIES merge (Resolving Interference When Merging Models): jondurbin/airoboros-l2-13b-2.2, elinas/chronos-13b-v2, NousResearch/Nous-Hermes-Llama2-13b, lemonilia/limarp-llama2-v2,   PygmalionAI/pygmalion-2-13b.

**Language-Vision models**

* LLaVA - trained on LLaMA 2. Current biggest version is [LLaVA-1.6-34B](https://huggingface.co/liuhaotian/llava-v1.6-34b), and LLaVA-NEXT has a [paper](https://llava-vl.github.io/blog/2024-01-30-llava-next/).
* BakLLaVA-1 - fine-tuned on Mistral


## LLMs / Lists and Ranking

* GitHub: [Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM)

* HF: [🤗 Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)
* Rentry: [Another LLM Roleplay Rankings](https://rentry.co/ALLMRR)
* Rentry: [Ayumi's LLM Role Play & ERP Ranking (NSFW)](https://rentry.co/ayumi_erp_rating)  - last updated 2023-11-21
* [BestERP](https://besterp.ai/s/models)
* [Rankings site for online NSFW chatbots](https://nsfw-chatbot-rankings.web.app/#/)
* [LLM Explorer](https://llm.extractum.io/) by Extractum
* Reddit: [Wiki by r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/wiki/models/)

For awareness, the scores are NOT representative of quality of prose, performance across the entire context window (i.e. ability to effectively recall information accurately), stability (i.e. logical flow, coherence) and actual RP performance. There are many models that score well that perform very poorly with actual use 
For example, in October 2023, Mythomax scores worse, but is better than a majority of the models that score better than it.

Recommendations for levels as of April 2024:
    <7B: Phi-3
    7b: Neural Chat V3, Mistral 7B (v0.3 - 22/05/2024), Llama 3.1 8B
    13b: Mythomax and its variants, Athena
    20b: Emerhyst, MLewd-remm-l2-chat, Beyonder 4x7B
    33b: Airoboros, Chronoboros
    45b: Mixtral 8x7B
    70b+: miqu-1-70b, Euryale Inverted L2, Xwin, Synthia 1.5 - 70B outperform GPT-3.5 and aim to rival GPT4. Llama3-70B (April 2024) outperforms GPT4 from April 2023.


## LLMs / UIs and WebUIs

Some of the UIs, like SillyTavern, also have APIs, that can be used for own coding projects and automation.

The full list of UIs can be found in [Deployment and UI](deployment-and-ui.md).

- [Oobabooga Text Generation WebUI](https://github.com/oobabooga/text-generation-webui) - For beginners, with a full package of chat features
- [Kobold.CPP](https://github.com/LostRuins/koboldcpp)
- [KoboldAI Client](https://github.com/KoboldAI/KoboldAI-Client)
- [TavernAI](https://github.com/TavernAI/TavernAI)
- [SillyTavern](https://docs.sillytavern.app/) - Power-user Front-End with a group chat capability, with SillyTavern Extras for things like image generation (so chars can send you selfies and photos) and voice generation
- [Agnaistic](https://agnai.chat/)
- [oterm](https://github.com/ggozad/oterm) - For those who prefer/need a CLI UI

## Personality specifications for AIs

Current generation of LLMs can have issues like repeatition and losing the character after a number of requests. This is currently being addressed by the community. 
*(As of Feb 2024)*

#### W++
The format example:

Personality ( "cute" + "gentle" + "intelligent" + "etc" ) Loves ( "food" + "etc" ) 

#### Natural language

