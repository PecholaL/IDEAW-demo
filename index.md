# IDEAW

## Abstract
<p align="justify">
Audio watermarking embeds messages into the audio and accurately extracts the watermark even after the watermarked audio has been damaged. Compared to traditional digital watermarking algorithms, neural watermarking using neural networks has better robustness against various attacks that are considered during the training process. However, neural watermarking methods suffer to low capacity. In addition, in practical scenarios, watermarks are redundantly embedded in audio according to the demand, and the audio is also subject to cropping and splicing, which makes the efficient locating of watermarks a problem worth exploring. In this paper, we use invertible neural network to realize a dual-embedding strategy, and at the same time, we consider the impact of the attack layer on the invertible neural network in robustness training and improve the model so as to enhance the reasonableness and stability. Experiment shows that the proposed model, IDEAW, can withstand various attacks and has higher capacity with more efficient locating ability compared to the state-of-the-art methods.
</p>

## Overview
<p align="justify">

</p>

![Model Architecture ](assets/IDEAW.png)
<p align="center">Figure.1 The Architecture of IDEAW.</p>
<p>&nbsp;</p> 

## Watermarked Audio Samples
Audio samples are taken from the VCTK corpus and FMA corpus. The capacity of **IDEAW** achieves 46 bits per second (maintaining SNR at about 30 dB).
What can a 46-bit watermark accomplish?

<script>
function pauseOthers(ele) {
    $("audio").not(ele).each(function (index, audio) {audio.pause();});
}
</script>


html <div align="center"> <img src="assets/wm_msg/I.png" width = 40 /> </div>
![wm_msg_1](assets/wm_msg/I.png) <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> 

![wm_msg_2](assets/wm_msg/D.png) <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> 

![wm_msg_3](assets/wm_msg/E.png) <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> 

![wm_msg_4](assets/wm_msg/A.png) <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> 

![wm_msg_5](assets/wm_msg/W.png) <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> 

<p>&nbsp;</p> 


## Waveform Samples

