# MAIN-VC

## Abstract
<p align="justify">
Audio watermarking embeds messages into the audio and accurately extracts the watermark even after the watermarked audio has been damaged. Compared to traditional digital watermarking algorithms, neural watermarking using neural networks has better robustness against various attacks that are considered during the training process. However, neural watermarking methods suffer to low capacity. In addition, in practical scenarios, watermarks are redundantly embedded in audio according to the demand, and the audio is also subject to cropping and splicing, which makes the efficient locating of watermarks a problem worth exploring. In this paper, we use invertible neural network to realize a dual-embedding strategy, and at the same time, we consider the impact of the attack layer on the invertible neural network in robustness training and improve the model so as to enhance the reasonableness and stability. Experiment shows that the proposed model, **IDEAW**, can withstand various attacks and has higher capacity with more efficient locating ability compared to the state-of-the-art methods.
</p>

## Overview
<p align="justify">

</p>

![Model Architecture ](assets/IDEAW.png)
<p align="center">Figure.1 The Architecture of IDEAW.</p>
<p>&nbsp;</p> 

## Watermarked Audio Samples
Audio samples are taken from the VCTK corpus and FMA corpus. The capacity of **IDEAW** reaches 46 bits per second.
What can a 46-bit watermark accomplish?

<script>
function pauseOthers(ele) {
    $("audio").not(ele).each(function (index, audio) {audio.pause();});
}
</script>


<audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> 



<p>&nbsp;</p> 


## Waveform Samples
