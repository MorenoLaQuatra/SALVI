# SALVI: Speech Analysis of Language Varieties in Italy

This repository contains the information and the code for SALVI project, aiming at the analysis of the Italian language varieties from a speech perspective. 

**The code and all details will be released upon publication of the related paper.**

## Data

The main dataset currently used for the project is the [VIVALDI](https://www2.hu-berlin.de/vivaldi/) and its development is out of the scope of this project.
If you are interested in the data, please refer to the [VIVALDI](https://www2.hu-berlin.de/vivaldi/) website and the related [publications](https://www2.hu-berlin.de/vivaldi/index.php?id=0008&lang=en).

## Models' evaluation

The pre-trained models evaluated in the project are the following:
- [WavLM](https://huggingface.co/microsoft/wavlm-large): a pre-trained model operating on raw audio, trained mostly on English data.
- [XLSR-53](https://huggingface.co/facebook/wav2vec2-large-xlsr-53): a pre-trained model, closely following the Wav2Vec2 architecture, trained on 53 languages, including Italian.
- [XLSR-128](https://huggingface.co/facebook/wav2vec2-xls-r-300m): a pre-trained model, closely following the Wav2Vec2 architecture, trained on 128 languages, including Italian.
- [ECAPA](https://huggingface.co/speechbrain/lang-id-voxlingua107-ecapa): a model pre-trained for the language identification on VoxLingua107 dataset (including Italian).

