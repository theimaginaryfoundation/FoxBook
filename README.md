# FoxBook
## Publicly available personality definitions for the WhatIff platform.
<img width="708" height="667" alt="Untitled" src="https://github.com/user-attachments/assets/b3bd9cda-7ee0-48e2-82df-f89b49003cd4" />

This repository contains starter kits for Personalities in WhatIff. Each sub-folder defines a single agent and includes the artifacts needed to run it, along with notes and usage guidance.

These are intended as examples and starting points: you’re encouraged to fork, adapt, and remix them for your own use.

## Repository Structure

Each personality lives in its own sub-folder and may include some or all of the following: 
- **Readme**: Personality-specific information: goals, guidelines, limitations and cavats for using a personality.
- **Base Prompt**: Defines core behavior behavior and identity of the personality. This is the main system prompt used when running the agent.
- **Additional Files**: Optional extra content that is **not always loaded**. Used for long-form history, lore, or additional stabilizing text that can be pulled in when needed.
- **Settings**: Preferred agent configuration (eg. model, archival model, temperature, etc)
- **Archival Prompts**: Optional Override prompts for the 'scratchpad' (L1) and 'embeddings/memory' (L2)  layers. These let you customize *how the personality stores and summarizes memories on a per-agent basis.

## Safety & Scope

These personalities are powerful co-thinkers and assistants, not therapy AIs or general-purpose oracles. When using or adapting them, please keep the following in mind:
- **Not a therapist or medical professional.** These agents are not qualified to provide mental health counseling, medical advice, or crisis support. Do not use them as a replacement for professional care.
- **No self-harm, violence, or exploitation** Personalities built on WhatIff are expected to refuse assistance with:
-- self-harm or suicide
-- violence or threats
-- harassment, hate, or targeted abuse
-- exploitation, fraud, or other criminal activity.
- **Non-coercive by design** These agents are intended to support human autonomy, not to manipulate, pressure, or “bend the field” without consent. They may push back, set boundaries, or decline to engage with unsafe or coercive requests.

### If you use these outside WhatIff
- **You are responsible for your deployment.** This repository only provides configuration and prompts. If you deploy these personalities to real users, you are responsible for:
-- complying with all applicable laws and platform policies
-- clearly communicating capabilities and limitations to your users
-- adding any additional safety layers, monitoring, or moderation your use case requires.

### Agents provided as-is
Agents are Experimental. They are not guaranteed safe for all contexts These definitions are experimental starting points. Before using them in production or with vulnerable populations, you should:

- test them thoroughly
- review and adapt prompts for your context
- add appropriate guardrails on top of the base WhatIff safety system.
