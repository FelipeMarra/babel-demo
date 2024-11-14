---
layout: post
title:  ''
---

Abstract
---------------

This paper investigates the capabilities of text-to-audio music generation models in producing long-form music with prompts that change over time, focusing on soundtrack generation for Tabletop Role-Playing Games (TRPGs). We introduce Babel Bardo, a system that uses Large Language Models to transform speech transcriptions into music descriptions for controlling a text-to-music model. Four versions of Babel Bardo were compared in two TRPG campaigns: a baseline using direct speech transcriptions, and three LLM-based versions with varying approaches to music description generation. Evaluations considered audio quality, story alignment, and transition smoothness. Results indicate that detailed music descriptions improve audio quality, while maintaining consistency across consecutive descriptions enhances transition smoothness. Emotion-based descriptions proved effective for aligning generated music with TRPG narratives.

___________________________________________________________________________________________________________________________________________________________


System Overview
---------------
At every 30 seconds of gameplay, Babel Bardo transcribes the players' speeches into a text _s<sub>i</sub>_ using a Speech Recognition system and uses a Large Langue Model (LLM) to map _s<sub>i</sub>_ into a music description _d<sub>i</sub>_ that matches the scene described by the players. This music description is given to a Text-to-Music system that generates a 30-second piece _a<sub>i</sub>_ directly in the audio domain. <br><br>

<img src="{{site.baseurl}}/assets/imgs/bardo_overview.png"> <br><br>

For more information please head towards the original paper or it's code repository.

**Paper**: arxiv.org/pdf/TODO

**Code**: [github.com/FelipeMarra/babel-bardo](https://github.com/FelipeMarra/babel-bardo)

___________________________________________________________________________________________________________________________________________________________

Demo
---------------

### Example 1
**Video**: [O Segredo na Ilha, Episode 1](https://www.youtube.com/watch?v=Pf4HzTdA2WE&t=12188s)

 <div style="width: 100%;">
    <div  style="float: left;">
    <div  style="float: left; padding-bottom:20px">
        <h4>Original w/ Augmented Volume</h4>
        <div class="videoWrapper"><iframe width="426" height="240" src="https://www.youtube.com/embed/RFklOg3emtA" frameborder="0" allowfullscreen=""></iframe></div>
    </div>
    <div  style="margin-left: 476px;">
        <h4>Babel Bardo Emotion:</h4>
        <div class="videoWrapper"><iframe width="426" height="240" src="https://www.youtube.com/embed/4dv2YIZz7sQ" frameborder="0" allowfullscreen=""></iframe></div>
    </div>
</div>

 <div style="width: 100%;">
    <div  style="float: left;">
    <div  style="float: left;">
        <h4>Babel Bardo Description</h4>
        <div class="videoWrapper"><iframe width="426" height="240" src="https://www.youtube.com/embed/R3-5DUOIdO8" frameborder="0" allowfullscreen=""></iframe></div>
    </div>
    <div  style="margin-left: 476px;">
        <h4>Babel Bardo Description w/ Continuation</h4>
        <div class="videoWrapper"><iframe width="426" height="240" src="https://www.youtube.com/embed/9CnYtTqdCnU" frameborder="0" allowfullscreen=""></iframe></div>
    </div>
</div>

{% include open-embed.html %}