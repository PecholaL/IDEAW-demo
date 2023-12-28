# IDEAW

## Abstract
<p align="justify">
Audio watermarking embeds messages into the audio and accurately extracts the watermark even after the watermarked audio has been damaged. Compared to traditional digital watermarking algorithms, neural watermarking using neural networks has better robustness against various attacks that are considered during the training process. However, neural watermarking methods suffer to low capacity. In addition, in practical scenarios, watermarks are redundantly embedded in audio according to the demand, and the audio is also subject to cropping and splicing, which makes the efficient locating of watermarks a problem worth exploring. In this paper, we use invertible neural network to realize a dual-embedding strategy, and at the same time, we consider the impact of the attack layer on the invertible neural network in robustness training and improve the model so as to enhance the reasonableness and stability. Experiment shows that the proposed model, IDEAW, can withstand various attacks and has higher capacity with more efficient locating ability compared to the state-of-the-art methods.
</p>

## Overview
<p align="justify">

</p>

<div style="text-align: center;">
<img src="assets/IDEAW.png" width = 1000 />
</div>
<p align="center">The Architecture of IDEAW.</p>
<p>&nbsp;</p> 

## Watermarked Audio Samples
Audio samples are taken from the VCTK corpus and FMA corpus. The capacity of **IDEAW** achieves 46 bits per second (maintaining SNR at about 30 dB).
### What can 46-bit watermarks accomplish?

<script>
function pauseOthers(ele) {
    $("audio").not(ele).each(function (index, audio) {audio.pause();});
}
</script>

##### · Embedding 7*6 binary figures into audios.
<img src="assets/wm_msg/I.png" width = 200 /> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> SNR = ??, ACC=??

<img src="assets/wm_msg/D.png" width = 200 /> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> SNR = ??, ACC=??

<img src="assets/wm_msg/E.png" width = 200 /> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> SNR = ??, ACC=??

<img src="assets/wm_msg/A.png" width = 200 /> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> SNR = ??, ACC=??

<img src="assets/wm_msg/W.png" width = 200 /> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> SNR = ??, ACC=??

##### · Embedding 5-bit encoded characters into audios. (46 bits watermark -> 9 characters)
Embedding "IDEAWOKAY" (01000-00100-00101-00001-10111-01111-01011-00001-11001-0) into audio.

"IDEAWOKAY" <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/wmd_audios/p227_003.mp3" type="audio/mpeg"></audio> SNR = ??, ACC = ??


<p>&nbsp;</p> 


## Waveform Samples
Waveforms of watermared audios and residual to host audios. The size of the embedded watermark defaults to 46 bits.

<div style="text-align: center;">
<img src="assets/wmd_waveforms/test.png" width = 500 />
</div>
<p align="center">(i) SNR=??</p>

<div style="text-align: center;">
<img src="assets/wmd_waveforms/test.png" width = 500 />
</div>
<p align="center">(ii) SNR=??</p>

<div style="text-align: center;">
<img src="assets/wmd_waveforms/test.png" width = 500 />
</div>
<p align="center">(iii) SNR=??</p>

<div style="text-align: center;">
<img src="assets/wmd_waveforms/test.png" width = 500 />
</div>
<p align="center">(iv) SNR=??</p>


# IDEAW Code
We will release our code as soon as the paper is accepted.
