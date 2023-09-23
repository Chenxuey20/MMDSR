<center><font size=4>(Submitted on ICASSP 2024)</font></center>

<center> <b><font size=4>Authors</font></b>: <i><font size=4>Xueyuan Chen, Yuejiao Wang, Xixin Wu, Disong Wang, Zhiyong Wu, Xunying Liu, Helen Meng</font></i> </center>

## 1. Abstract

Dysarthric speech reconstruction (DSR) aims to transform dysarthric speech into normal speech by improving the intelligibility and naturalness. This is a challenging task especially for patients with severe dysarthria and speaking in complex, noisy acoustic environments. To address these challenges, we propose a novel multi-modal framework to utilize visual information, e.g., lip movements, in DSR as extra clues for reconstructing the highly abnormal pronunciations. The multi-modal framework consists of: (i) a multi-modal encoder to extract robust phoneme embeddings from dysarthric speech with auxiliary visual features; (ii) a variance adaptor to infer the normal phoneme duration and pitch contour from the extracted phoneme embeddings; (iii) a speaker encoder to encode the speaker’s voice characteristics; and (iv) a mel-decoder to generate the reconstructed mel-spectrogram based on the extracted phoneme embeddings, prosodic features and speaker embeddings. Both objective and subjective evaluations conducted on the commonly used UASpeech corpus show that our proposed approach can achieve significant improvements over baseline systems in terms of speech intelligibility and naturalness, especially for the speakers with more severe symptoms. Compared with original dysarthric speech, the reconstructed speech achieves 42.1% absolute word error rate reduction for patients with more severe dysarthria levels.

## 2. Proposed model architecture

<img src="./wavs/model_architecture.png" width="100%">

## 3. Audio samples of different model settings

- **Original**: the original dysarthric speech.
- **A-DSR**: The audio-only encoder (described in paper 2.1.1) is used for the DSR model.
- **AV-DSR (Proposed)**: The VGG-based audio-visual encoder (described in paper 2.1.2) is used for the DSR model.
- **AVHuBERT-DSR (Proposed)**: The AV-HuBERT-based audio-visual encoder (described in paper 2.1.3) is used for the DSR model.

