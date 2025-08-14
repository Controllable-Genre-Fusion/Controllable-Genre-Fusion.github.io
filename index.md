# Fine-Grained control over Music Generation with Activation Steering

Tags: AI

# Abstract

We present a method for fine-grained control over music generation through inference-time interventions on an autoregressive generative music transformer called MusicGen. Our approach enables timbre transfer, style transfer, and genre fusion by steering the residual stream using weights of linear probes trained on it, or by steering the attention layer activations in a similar manner. We observe that modelling this as a regression task provides improved performance, hypothesizing that the mean-squared-error better preserve meaningful directional information in the activation space. Combined with the global conditioning offered by text prompts in MusicGen, our method provides both global and local control over music generation.

Check out our paper

[Fine-Grained control over Music Generation with Activation Steering](https://arxiv.org/abs/2506.10225)

# Samples

To demonstrate our method, we start with a sample of a trumpet playing a western classical piece.

[og_audio.wav](outputs/og_audio.wav)

And we were able to change the ‘style’/ genre:

To electronic:

[classical_elec.wav](outputs/classical_elec.wav)

To rock:

[elec_Rock.wav](outputs/elec_Rock.wav)

Or to add a tabla accompaniment at the tempo of the melodic sample:

[rock_indian (1).wav](outputs/rock_indian_(1).wav)

And we were also able to change instruments:

To violin:

[to_violin.wav](outputs/to_violin.wav)

To xylophone:

[to_xylophone.wav](outputs/to_xylophone.wav)

Our method involves intervention during inference time, for example, in the following audio sample, we intervene in the activations at the 5th second and the change in audio is evident.

[download (1).wav](outputs/download_(1).wav)

## Additional Samples

Original (rock):

[rock_first10s.wav](outputs/rock_first10s.wav)

After steering (adding pop)

[rock_to_pop_5.wav](outputs/rock_to_pop_5.wav)

Original (pop):

[pop_first10s.wav](outputs/pop_first10s.wav)

After steering

[pop_to_rock_1.wav](outputs/pop_to_rock_1.wav)

[pop_to_rock_3.wav](outputs/pop_to_rock_3.wav)

Original (hip-hop)

[hiphop_first10s.wav](outputs/hiphop_first10s.wav)

After steering (adding folk):

[hip-hop_to_folk_1.wav](outputs/hip-hop_to_folk_1.wav)

MusicGen (https://arxiv.org/abs/2306.05284) is an auto-regressive music transformer. We intervene with the activations in the residual stream or at the outputs of the attention layer to achieve fine-grained control over music generation.

[](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfeVmaDwEydRw21eHyYXCJF9eqt-hCl64632Tl7WKv75bRznbzIN_vVs1Jve8xFAEQdyPuYh7p-BSXUGbdpHa2Piwn1PQiP0dCF4O4onftGjp5c4CicycU50XFBBxpiGLapCeUwsw?key=IchWhVE9EcgkypeuEzw3rZIx)