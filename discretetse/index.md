# Generative-based Target Speech Extraction with Speech Discretization and Vocoder
## Abstract
Target speech extraction (TSE) aims to extract the target speaker's speech from a mixture recording with the help of an auxiliary target speaker's speech. 
Most existing TSE method use a discriminative-based model to predict the proportion of the target speaker in a mixture speech, but discriminative-based model suffers from the problem of not being able to remove residual interfering speech. 
In this paper, we combine the  speech discretization and vocoder techniques to propose a generation-based TSE approach. 
By utilizing the vocoder with the input of discrete symbols, after the prediction of discrete symbol sequence with the help of an auxiliary input, the target speech could be re-synthesized. 
Experiments on the WSJ0-2mix-extr and Libri2mix show that our proposed method can obtain high quality target speech without interference.


## Test samples of Target Speech Extraction 
The sound files blow are some raw noisy wavs and the extracted speech from different methods.
All the samples are driven from the test set of Libri2Mix (16k min).

**(1) Sample1:**

Noisy wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-noisy.wav?raw=true"></audio>

Reference wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-ref.wav?raw=true"></audio>

DPCCN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-dpccn.wav?raw=true"></audio>

Our discrete extraction:

(UniCATs-HuBERT-512)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-hubert512.wav?raw=true"></audio>
(UniCATs-HuBERT-4096)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-hubert4096.wav?raw=true"></audio>
(UniCATs-vq-wav2vec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-vq.wav?raw=true"></audio>
(encodec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample1-enc.wav?raw=true"></audio>
\\

**(2) Sample2:**

Noisy wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-noisy.wav?raw=true"></audio>

Reference wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-ref.wav?raw=true"></audio>

DPCCN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-dpccn.wav?raw=true"></audio>

Our discrete extraction:

(UniCATs-HuBERT-512)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-hubert512.wav?raw=true"></audio>
(UniCATs-HuBERT-4096)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-hubert4096.wav?raw=true"></audio>
(UniCATs-vq-wav2vec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-vq.wav?raw=true"></audio>
(encodec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample3-enc.wav?raw=true"></audio>
\\

**(3) Sample3:**

Noisy wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-noisy.wav?raw=true"></audio>

Reference wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-ref.wav?raw=true"></audio>

DPCCN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-dpccn.wav?raw=true"></audio>

Our discrete extraction:

(UniCATs-HuBERT-512)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-hubert512.wav?raw=true"></audio>
(UniCATs-HuBERT-4096)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-hubert4096.wav?raw=true"></audio>
(UniCATs-vq-wav2vec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-vq.wav?raw=true"></audio>
(encodec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample4-enc.wav?raw=true"></audio>
\\

**(4) Sample4:**

Noisy wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-noisy.wav?raw=true"></audio>

Reference wav:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-ref.wav?raw=true"></audio>

DPCCN:
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-dpccn.wav?raw=true"></audio>

Our discrete extraction:

(UniCATs-HuBERT-512)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-hubert512.wav?raw=true"></audio>
(UniCATs-HuBERT-4096)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-hubert4096.wav?raw=true"></audio>
(UniCATs-vq-wav2vec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-vq.wav?raw=true"></audio>
(encodec)
<audio id="audio" controls="" preload="none">
<source id="wav" src="https://github.com/earthmanylf/earthmanylf.github.io/blob/main/discretetse/wavs/sample5-enc.wav?raw=true"></audio>