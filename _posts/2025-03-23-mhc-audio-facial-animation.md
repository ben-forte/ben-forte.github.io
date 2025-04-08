---
title: 'Metahuman'
date: 2025-03-23
permalink: /posts/ue-metahuman-audio-facial-animation
tags:
  - metahuman
  - unreal engine
---

Metahuman
======
This video showcases my early experiments with audio-driven facial animation using Unreal Engine 5.5's MetaHuman capabilities. 
I focused on exaggerated articulation to observe the lip-sync accuracy of Unreal Engine MetaHuman.

Audio-Facial Animation
------
"Unreal Engine 5.5: MetaHuman Audio to Facial Animation (Exaggerated Articulation)"
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/TdYFo9or-Hw/0.jpg)](https://www.youtube.com/watch?v=TdYFo9or-Hw) <br>
### Subtitle
> Bob brought bright blue balloons to the big birthday bash. 
>
> Peter Piper picked a peck of pickled peppers. 
> 
> We saw a flock of fluffy finches flying in the field. 
>
> The very vivid violets vanished from the vase. 
> 
> Many merry monkeys munch mangoes in Madagascar.



### Steps
1. Text Generation: Used Gemini 2.0 Flash mLLM to create a paragraph with extreme lip movements. The text uses a lot of words starting with the letters <kbd>B</kbd>, <kbd>P</kbd>, <kbd>F</kbd>, <kbd>V</kbd>, <kbd>M</kbd> which require distinct lip movements.
2. Audio Recording: Recorded the generated text using [Natural Reader](https://www.naturalreaders.com/) (text-to-speech) to capture clear audio.
3. MetaHuman Creation: Designed a MetaHuman named 'Sook-ja' in MetaHuman Creator (MHC).
4. Audio Application: Applied the recorded audio to Sook-ja's facial mesh within Unreal Engine 5.5.

To truly appreciate the exaggerated articulation, feel free to enable subtitles and try speaking along! 🙂 
You can also see the facial control rig in action [here](https://youtu.be/JMbK1a-bpSo)

This project is part of my effort to enhance my Unreal Engine skills, building upon my previous experience as part of my PhD work in simulating construction environments (see [my portfolio](https://bit.ly/ts-portfolio-ue-unity-videos)).

My next step is to explore adding emotional nuances to the facial animation. I'm particularly interested in the research presented in:
Pan, Ye, et al. "VASA-Rig: Audio-Driven 3D Facial Animation with ‘Live’Mood Dynamics in Virtual Reality." IEEE Transactions on Visualization and Computer Graphics (2025).
This paper explores how to capture and translate emotional cues from audio into realistic facial expressions. (see: https://ieeexplore.ieee.org/document/10916977)


As I'm relatively new to MetaHuman facial animation, any feedback, tips, or suggestions are greatly appreciated! 

#UnrealEngine #MetaHuman #MetaHumanCreator #MHC #FacialAnimation #AudioDriven #3DAnimation #VirtualReality #Innovation #Portfolio #DigitalHumans #LLM


References
------
[1] Jack Saunders, [Unreal Engine 5.5 MetaHuman Audio To Facial Animation Tutorial](https://medium.com/@jacksaunders909/wav2lip-generalized-lip-sync-models-e0effc4e8ed3) <br>
[2] Text to speech, [Natural reader](https://www.naturalreaders.com/online/) <br>
[3] Epic Games, [Audio Driven Animation for MetaHuman](https://dev.epicgames.com/documentation/en-us/metahuman/audio-driven-animation-for-metahuman)<br>