---
layout: default
title: Genre Fusion via Activation Steering
---

<style>
.sample-pair {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 1rem 0;
  flex-wrap: wrap;
}
.sample-block {
  display: flex;
  flex-direction: column;
  align-items: center;
  min-width: 220px;
}
.sample-caption {
  font-size: 0.9rem;
  margin-top: 0.35rem;
  color: #444;
}
.arrow {
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 80px;
}
.arrow svg {
  width: 64px;
  height: 32px;
}
.legend {
  font-size: 0.9rem;
  color: #666;
  margin-bottom: 0.75rem;
}
</style>

# Abstract

Computational Music Generation is evolving towards non-conventional styles, demanding methods that enable precise and controllable blending of diverse music elements. In this work, we present a method for fine grained control using inference time-interventions on an autoregressive generative transformer, MusicGen. Through our approach, we achieve genre fusion by steering the residual stream using weights of a linear probe on it.

# Samples

To demonstrate our method, we start with a sample of music in a certain genre, and transition it into the second genre.

<div class="legend">
Original → Steered (we apply activation steering to move the audio from the left genre towards the right genre)
</div>

---

### Classical to Electronic
---

<div class="sample-pair">
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/classical_electronic_1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <div class="sample-caption">Classical (original)</div>
  </div>

  <div class="arrow" aria-hidden="true">
    <svg viewBox="0 0 24 12" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 6h18" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M12 0l6 6-6 6" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </div>

  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/classical_electronic_steered_1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <div class="sample-caption">Electronic (steered)</div>
  </div>
</div>

<div class="sample-pair">
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/classical_electronic_2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <div class="sample-caption">Classical (original)</div>
  </div>

  <div class="arrow" aria-hidden="true">
    <svg viewBox="0 0 24 12" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 6h18" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M12 0l6 6-6 6" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </div>

  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/classical_electronic_steered_2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <div class="sample-caption">Electronic (steered)</div>
  </div>
</div>

<div class="sample-pair">
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/classical_electronic_3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <div class="sample-caption">Classical (original)</div>
  </div>

  <div class="arrow" aria-hidden="true">
    <svg viewBox="0 0 24 12" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 6h18" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M12 0l6 6-6 6" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </div>

  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/classical_electronic_steered_3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <div class="sample-caption">Electronic (steered)</div>
  </div>
</div>

---

### Electronic to Jazz
---

<div class="sample-pair">
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/electronic_jazz_1.wav" type="audio/wav">
    </audio>
    <div class="sample-caption">Electronic (original)</div>
  </div>
  <div class="arrow" aria-hidden="true">
    <svg viewBox="0 0 24 12" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 6h18" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M12 0l6 6-6 6" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </div>
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/electronic_jazz_steered_1.wav" type="audio/wav">
    </audio>
    <div class="sample-caption">Jazz (steered)</div>
  </div>
</div>

---

### Jazz to Rock
---

<div class="sample-pair">
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/jazz_rock_1.wav" type="audio/wav">
    </audio>
    <div class="sample-caption">Jazz (original)</div>
  </div>
  <div class="arrow" aria-hidden="true">
    <svg viewBox="0 0 24 12" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 6h18" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M12 0l6 6-6 6" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </div>
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/jazz_rock_steered_1.wav" type="audio/wav">
    </audio>
    <div class="sample-caption">Rock (steered)</div>
  </div>
</div>

---

### Rock to Classical
---

<div class="sample-pair">
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/rock_classical_1.wav" type="audio/wav">
    </audio>
    <div class="sample-caption">Rock (original)</div>
  </div>
  <div class="arrow" aria-hidden="true">
    <svg viewBox="0 0 24 12" xmlns="http://www.w3.org/2000/svg">
      <path d="M0 6h18" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round"/>
      <path d="M12 0l6 6-6 6" stroke="#333" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
    </svg>
  </div>
  <div class="sample-block">
    <audio controls preload="metadata">
      <source src="outputs/rock_classical_steered_1.wav" type="audio/wav">
    </audio>
    <div class="sample-caption">Classical (steered)</div>
  </div>
</div>

---

MusicGen ([paper link](https://arxiv.org/abs/2306.05284)) is an auto-regressive music transformer.  
We intervene with the activations in the residual stream or at the outputs of the attention layer to achieve fine-grained control over music generation.
