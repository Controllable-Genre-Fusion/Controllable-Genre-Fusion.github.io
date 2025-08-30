---
layout: default
title: Genre Fusion via Activation Steering
---

# Abstract

We present a method for fine-grained control over music generation through inference-time interventions on an autoregressive generative music transformer called MusicGen. Our approach enables timbre transfer, style transfer, and genre fusion by steering the residual stream using weights of linear probes trained on it, or by steering the attention layer activations in a similar manner. We observe that modelling this as a regression task provides improved performance, hypothesizing that the mean-squared-error better preserve meaningful directional information in the activation space. Combined with the global conditioning offered by text prompts in MusicGen, our method provides both global and local control over music generation.

# Samples

To demonstrate our method, we start with a sample of music in a certain genre, and transition it into the second genre.

### Rock to Classical
---

<audio controls preload="metadata">
  <source src="outputs/rock-to-classical.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/rock-to-classical-2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/rock-to-classical-3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/rock-to-classical-4.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/rock-to-classical-5.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

### Classical to Electronic
---
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_01.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/classical_electronic_02.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/classical_electronic_11.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/classical_electronic_12.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/classical_electronic_14.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/classical_electronic_18.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/classical_electronic_20.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

### Electronic to Jazz
---
<audio controls preload="metadata">
  <source src="outputs/elec2jazz_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/elec2jazz_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/elec2jazz_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/elec2jazz_4.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/elec2jazz_5.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/elec2jazz_6.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

### Jazz to Rock 
---

<audio controls preload="metadata">
  <source src="outputs/jazz_rock_01.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<audio controls preload="metadata">
  <source src="outputs/jazz_rock_02.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

MusicGen (https://arxiv.org/abs/2306.05284) is an auto-regressive music transformer. We intervene with the activations in the residual stream or at the outputs of the attention layer to achieve fine-grained control over music generation.

[](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfeVmaDwEydRw21eHyYXCJF9eqt-hCl64632Tl7WKv75bRznbzIN_vVs1Jve8xFAEQdyPuYh7p-BSXUGbdpHa2Piwn1PQiP0dCF4O4onftGjp5c4CicycU50XFBBxpiGLapCeUwsw?key=IchWhVE9EcgkypeuEzw3rZIx)