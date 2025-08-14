---
layout: default
title: Fine-Grained Control over Music Generation
---

# Fine-Grained control over Music Generation with Activation Steering

Tags: AI

# Abstract

We present a method for fine-grained control over music generation through inference-time interventions on an autoregressive generative music transformer called MusicGen. Our approach enables timbre transfer, style transfer, and genre fusion by steering the residual stream using weights of linear probes trained on it, or by steering the attention layer activations in a similar manner. We observe that modelling this as a regression task provides improved performance, hypothesizing that the mean-squared-error better preserve meaningful directional information in the activation space. Combined with the global conditioning offered by text prompts in MusicGen, our method provides both global and local control over music generation.

Check out our paper

[Fine-Grained control over Music Generation with Activation Steering](https://arxiv.org/abs/2506.10225)

# Samples

To demonstrate our method, we start with a sample of a trumpet playing a western classical piece.

---

<audio controls preload="metadata">
  <source src="outputs/og_audio.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

And we were able to change the style/ genre:

To electronic:
<audio controls preload="metadata">
  <source src="outputs/classical_elec.wav" type="audio/wav">
</audio>

To rock:
<audio controls preload="metadata">
  <source src="outputs/elec_Rock.wav" type="audio/wav">
</audio>

Or to add a tabla accompaniment at the tempo of the melodic sample:

<audio controls preload="metadata">
  <source src="outputs/rock_indian_(1).wav" type="audio/wav">
</audio>

And we were also able to change instruments:

To violin:

<audio controls preload="metadata">
  <source src="outputs/to_violin.wav" type="audio/wav">
</audio>

To xylophone:

<audio controls preload="metadata">
  <source src="outputs/to_xylophone.wav" type="audio/wav">
</audio>

Our method involves intervention during inference time, for example, in the following audio sample, we intervene in the activations at the 5th second and the change in audio is evident.

<audio controls preload="metadata">
  <source src="outputs/download_(1).wav" type="audio/wav">
</audio>

---

## Additional Samples

Original (rock):

<audio controls preload="metadata">
  <source src="outputs/hip-hop_to_folk_1.wav" type="audio/wav">
</audio>

After steering (adding pop)

<audio controls preload="metadata">
  <source src="outputs/rock_to_pop_5.wav" type="audio/wav">
</audio>

Original (pop):

<audio controls preload="metadata">
  <source src="outputs/pop_first10s.wav" type="audio/wav">
</audio>

After steering
<audio controls preload="metadata">
  <source src="outputs/pop_to_rock_1.wav" type="audio/wav">
</audio>

<audio controls preload="metadata">
  <source src="outputs/pop_to_rock_3.wav" type="audio/wav">
</audio>

Original (hip-hop)

<audio controls preload="metadata">
  <source src="outputs/hiphop_first10s.wav" type="audio/wav">
</audio>

After steering (adding folk):

<audio controls preload="metadata">
  <source src="outputs/hip-hop_to_folk_1.wav" type="audio/wav">
</audio>

MusicGen (https://arxiv.org/abs/2306.05284) is an auto-regressive music transformer. We intervene with the activations in the residual stream or at the outputs of the attention layer to achieve fine-grained control over music generation.

[](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfeVmaDwEydRw21eHyYXCJF9eqt-hCl64632Tl7WKv75bRznbzIN_vVs1Jve8xFAEQdyPuYh7p-BSXUGbdpHa2Piwn1PQiP0dCF4O4onftGjp5c4CicycU50XFBBxpiGLapCeUwsw?key=IchWhVE9EcgkypeuEzw3rZIx)