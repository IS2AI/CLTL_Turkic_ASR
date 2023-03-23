# Speech Recognition for Turkic Languages Using Cross-Lingual Transfer Learning from Kazakh


This repository contains links to (1) [weights](https://drive.google.com/drive/folders/1KgfuqCKerapO_v9Ts1gic42EFrib1zNN?usp=sharing) for automatic speech recognition (ASR) models built by applying cross-lingual transfer learning from Kazakh to nine lower-resourced Turkic languages (Azerbaijani, Bashkir, Chuvash, Kyrgyz, Sakha, Tatar, Turkish, Uyghur, and Uzbek) and (2) [pre-trained language models](https://drive.google.com/drive/folders/11mIYFEedsL2UtPcK5FT2cEy8rdcqxe39?usp=sharing).


## Recipe

Our project is built upon [ESPnet](https://github.com/espnet/espnet). To run the project, you should first follow all the steps in the [installation guide](https://espnet.github.io/espnet/installation.html).
Our code utilizes the [Commonvoice recipe](https://github.com/espnet/espnet/tree/master/egs2/commonvoice/asr1) from the ESPnet repository. Please remember to refer to it when building your own solution.


## Inference

To decode a single audio file, specify the paths to the (1) language model, (2) cepstral mean and variance normalization (CMVN), and (3) recognition_model files in the script `recog_wav.sh`:

```
lang_model = the path to the pre-trained language model
cmvn = the path to cmvn.ark (for example, data/train/cmvn.ark)
recog_model = the path to the pre-trained recognition model (can be downloaded from the link above)
```
And run the script with the path to the audio file specified:

```
./recog_wav.sh <path-to-audio-file>
```

## Video on YouTube

[LINK TO VIDEO GOES HERE]

## Citation

```bibtex
@INPROCEEDINGS{10066768,
  author={Orel, Daniil and Yeshpanov, Rustem and Varol, Huseyin Atakan},
  booktitle={2023 IEEE International Conference on Big Data and Smart Computing (BigComp)}, 
  title={Speech Recognition for Turkic Languages Using Cross-Lingual Transfer Learning from Kazakh}, 
  year={2023},
  volume={},
  number={},
  pages={174-182},
  doi={10.1109/BigComp57234.2023.00037}}
```
