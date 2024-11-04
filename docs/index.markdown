---
layout: home
title:  "Babel Bardo Demo"
---

Abstract
---------------

This paper investigates the capabilities of text-to-audio music generation models in producing long-form music with prompts that change over time, focusing on soundtrack generation for Tabletop Role-Playing Games (TRPGs). We introduce Babel Bardo, a system that uses Large Language Models to transform speech transcriptions into music descriptions for controlling a text-to-music model. Four versions of Babel Bardo were compared in two TRPG campaigns: a baseline using direct speech transcriptions, and three LLM-based versions with varying approaches to music description generation. Evaluations considered audio quality, story alignment, and transition smoothness. Results indicate that detailed music descriptions improve audio quality, while maintaining consistency across consecutive descriptions enhances transition smoothness. Emotion-based descriptions proved effective for aligning generated music with TRPG narratives.

<img src="{{site.baseurl}}/assets/imgs/bardo_overview.png">

**Code**: [github.com/FelipeMarra/babel-bardo](https://github.com/FelipeMarra/babel-bardo)

Demo
---------------

{{site.baseurl}}/assets/audio/test.wav


{% include open-embed.html %}