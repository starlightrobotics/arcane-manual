# ARCANE Manual: **A**I **R**ole-playing **C**hatbots **A**nd **N**ovel **E**ntities
#### Curated manual of Awesome Role-playing Censored and Uncensored models and chatbots
*by Starlight Robotics*

ARCANE Manual is a curated repository of AI Role-playing LLMs, chatbots, services, apps, interfaces, offline tools, and hardware tips. This manual provides insight for where to start, and reference links for seasoned developers.

To suggest the updates or edits, contact me on [Reddit](https://www.reddit.com/r/starlightrobotics/) or [Discord](https://discord.gg/zarD7dweKz).

[Hardware](hardware.md) is needed to run LLMs locally.

[Deployment](deployment.md) of your own LLM.

[Online services and apps](online-services.md) are available, paid and free.

[Chatbot Frameworks](chatbot-frameworks.md) for public presence.

[Challenges and Limits](challenges.md)

Image generation models can be found on [CivitAI](https://civitai.com/)

## LLMs / Models

* [PygmalionAI](https://github.com/PygmalionAI) - 
All models: [HuggingFace](https://huggingface.co/PygmalionAI), Most popular of which as of October 2023 is [Mythalion 13B](https://huggingface.co/PygmalionAI/mythalion-13b) - A merge of Pygmalion-2 13B and MythoMax 13B

* [MythoMax 13B](https://huggingface.co/Gryphe/MythoMax-L2-13b) - by Gryphe. Uncensored.

* [Manticore-13B](https://huggingface.co/mindrage/Manticore-13B-Chat-Pyg-Guanaco-GGML) - Uncensored.

* [SynthIA](https://huggingface.co/TheBloke/Synthia-7B-v1.3-GGUF) - Uncensored, trained on Mistral

* [CalliopeDS](https://huggingface.co/Doctor-Shotgun/CalliopeDS-L2-13B) - This is a Llama 2-based model consisting of a merge of several models using a weight-adjusted TIES merge (Resolving Interference When Merging Models): jondurbin/airoboros-l2-13b-2.2, elinas/chronos-13b-v2, NousResearch/Nous-Hermes-Llama2-13b, lemonilia/limarp-llama2-v2,   PygmalionAI/pygmalion-2-13b.

## LLMs / Lists and Ranking

* [🤗 Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

* [Another LLM Roleplay Rankings](https://rentry.co/ALLMRR)

* [Ayumi's LLM Role Play & ERP Ranking (NSFW)](https://rentry.co/ayumi_erp_rating)

* [Wiki by r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/wiki/models/)

For awareness, the scores are NOT representative of quality of prose, performance across the entire context window (i.e. ability to effectively recall information accurately), stability (i.e. logical flow, coherence) and actual RP performance. There are many models that score well that perform very poorly with actual use 
For example, in October 2023, Mythomax scores worse, but is better than a majority of the models that score better than it.

Recommendations for levels:

    7b: Mistral and its variants, especially Mistral-OpenOrca and Mistral-instruct
    13b: Mythomax and its variants, Athena
    33b: Airoboros, Chronoboros
    20b: Emerhyst, MLewd-remm-l2-chat
    70b+: Xwin, Synthia 1.2

Models for coding can be found in [⭐ Big Code Models Leaderboard](https://huggingface.co/spaces/bigcode/bigcode-models-leaderboard).

## LLMs / UIs and WebUIs

#### [Kobold.CPP](https://github.com/LostRuins/koboldcpp)
 <details>
  <summary>Details</summary>
      KoboldCpp is an easy-to-use AI text-generation software for GGML models. It's a single self contained distributable from Concedo, that builds off llama.cpp, and adds a versatile Kobold API endpoint, additional format support, backward compatibility, as well as a fancy UI with persistent stories, editing tools, save formats, memory, world info, author's note, characters, scenarios and everything Kobold and Kobold Lite have to offer.
</details>


#### [KoboldAI Client](https://github.com/KoboldAI/KoboldAI-Client)
 <details>
  <summary>Details</summary>
From providing user donated backends as workers, and providing an application interface for running all sort of models - it is PygmalionAI's pick for running models locally.

Discord: [KoboldAI](https://koboldai.org/discord)

Website: [KoboldAI](https://koboldai.org/pygmalion)
</details>

#### [TavernAI](https://github.com/TavernAI/TavernAI)
 <details>
  <summary>Details</summary>
The original frontend. It lacks the options for the user on their chatting experience, however it is still very usable.
</details>

#### [Oobabooga Text Generation WebUI](https://github.com/oobabooga/text-generation-webui)
 <details>
  <summary>Details</summary>
Oobabooga is a web interface, in the same look as Stable Diffusion Web UI by Automatic1111. It has more features, and compatibility compared to KoboldAI running models locally.

Discord: [Oobabooga](https://discord.gg/WKkMQYB4zu)
</details>

#### [SillyTavern](https://docs.sillytavern.app/)
 <details>
  <summary>Details</summary>
An open-source frontend for running LLM models. Provides all the tools to customize your chatting experience. An extensive modification of TavernAI.

Discord: [SillyTavern](https://discord.gg/sillytavern)
</details>

#### [Agnaistic](https://agnai.chat/)
 <details>
  <summary>Details</summary>
An open-source web based AI agnostic roleplay chat. The backend for chats: NovelAI, Horde, or other services. It can be ran locally, or use the production website.

Discord: [Agnaistic (link broken)](https://discord.gg/luminai)
</details>

## Personality specifications for AIs

Sample prompts and character sheets by [Botprompts](https://botprompts.net/)

#### W++
The format example:

Personality ( "cute" + "gentle" + "intelligent" + "etc" ) Loves ( "food" + "etc" ) 

#### Natural language

