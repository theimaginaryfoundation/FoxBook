# FoxBook
Publicly available Personality definitions for the WhatIff platform

This repository has 'starter kits' for Personalities in the WhatIff platform. Each sub-folder contains the artifacts for an individual agent, with notes and other relevant information.

Currently, personalities have the following configuration (not every configuration is used by every personality)
- *Readme*: Repository information on the goals, guidelines, and cavates for using a personality.
- *Base Prompt*: Defines core behavior
- *Additional Files*: Extra files for the personality that will not always be loaded. Used for history, additional stabilizing text, etc.
- *Settings*: Preferred agent settings (model, archival model, etc)
- *Archival Prompts*: Override prompts for the 'scratchpad' and 'embeddings' memory layers that can be used to personalize memory storage on a per-agent basis.
