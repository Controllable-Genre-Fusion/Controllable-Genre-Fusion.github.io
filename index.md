---
layout: default
title: Genre controlled music generation via Activation Steering
---

# Abstract

Computational Music Generation is evolving towards non-conventional styles, demanding methods that enable precise and controllable blending of diverse music elements. In this work, we present a method for fine-grained control using inference-time interventions on an autoregressive generative transformer, MusicGen. Through our approach, we achieve genre fusion by steering the residual stream using weights of a linear probe on it.

# Samples

To demonstrate our method, we start with a sample of music in a certain genre, and transition it into the second genre.

---

## Classical to Electronic
---

<table>
<tr>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_steered_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_steered_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/classical_electronic_steered_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>
</table>

---

## Electronic to Jazz
---

<table>
<tr>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/electronic_jazz_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/electronic_jazz_steered_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/electronic_jazz_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/electronic_jazz_steered_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/electronic_jazz_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/electronic_jazz_steered_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>
</table>

---

## Jazz to Rock
---

<table>
<tr>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/jazz_rock_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/jazz_rock_steered_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/jazz_rock_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/jazz_rock_steered_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/jazz_rock_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/jazz_rock_steered_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>
</table>

---

## Rock to Classical
---

<table>
<tr>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/rock_classical_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center" width="50%">
<audio controls preload="metadata">
  <source src="outputs/rock_classical_steered_1.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/rock_classical_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/rock_classical_steered_2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>

<tr>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/rock_classical_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Prompted</b>
</td>
<td align="center">
<audio controls preload="metadata">
  <source src="outputs/rock_classical_steered_3.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio><br>
<b>Steered</b>
</td>
</tr>
</table>

---

MusicGen ([https://arxiv.org/abs/2306.05284](https://arxiv.org/abs/2306.05284)) is an auto-regressive music transformer.  
We intervene with the activations in the residual stream or at the outputs of the attention layer to achieve fine-grained control over music generation.