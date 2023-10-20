# SALVI: Speech Analysis of Language Varieties in Italy

This repository contains the information and the code for SALVI project, aiming at the analysis of the Italian language varieties from a speech perspective. 

**The code and all details will be released upon publication of the related paper.**

## Data

The main dataset currently used for the project is the [VIVALDI](https://www2.hu-berlin.de/vivaldi/) and its development is out of the scope of this project.

| Region name (EN)      |    Region name (IT)   | \# cities | Included | Acronym |
|-----------------------|:---------------------:|:---------:|:--------:|:-------:|
| Abruzzo               |        Abruzzo        |     10    |     ✅    |  `abr`  |
| Basilicata            |       Basilicata      |     14    |     ✅    |  `bas`  |
| Calabria              |        Calabria       |     4     |     ✅    |  `cal`  |
| Campania              |        Campania       |     1     |     ❌    |  `cam`  |
| Emilia-Romagna        |     Emilia-Romagna    |     3     |     ✅    |  `eml`  |
| Friuli-Venezia Giulia | Friuli-Venezia Giulia |     28    |     ✅    |  `fvg`  |
| Lazio                 |         Lazio         |     1     |     ❌    |  `laz`  |
| Liguria               |        Liguria        |     14    |     ✅    |  `lig`  |
| Lombardy              |       Lombardia       |     25    |     ✅    |  `lom`  |
| Marche                |         Marche        |     0     |     ❌    |  `mar`  |
| Molise                |         Molise        |     17    |     ✅    |  `mol`  |
| Piedmont              |        Piemonte       |     24    |     ✅    |  `pie`  |
| Apulia                |         Puglia        |     10    |     ✅    |  `pug`  |
| Sardinia              |        Sardegna       |     19    |     ✅    |  `sar`  |
| Sicily                |        Sicilia        |     16    |     ✅    |  `sic`  |
| Tuscany               |        Toscana        |     10    |     ✅    |  `tos`  |
| Trentino-South Tyrol  |  Trentino Alto Adige  |     32    |     ✅    |  `tre`  |
| Umbria                |         Umbria        |     14    |     ✅    |  `umb`  |
| Aosta Valley          |     Valle d'Aosta     |     10    |     ✅    |  `vda`  |
| Veneto                |         Veneto        |     35    |     ✅    |  `ven`  |

This table shows the regions included in the dataset, the number of cities for each region, and the acronym used in the project.
Regions with having less than 3 cities are not included in the dataset (Campania, Lazio, Marche).


If you are interested in the data, please refer to the [VIVALDI](https://www2.hu-berlin.de/vivaldi/) website and the related [publications](https://www2.hu-berlin.de/vivaldi/index.php?id=0008&lang=en).

## Models' evaluation

The pre-trained models evaluated in the project are the following:
- [WavLM](https://huggingface.co/microsoft/wavlm-large): a pre-trained model operating on raw audio, trained mostly on English data.
- [XLSR-53](https://huggingface.co/facebook/wav2vec2-large-xlsr-53): a pre-trained model, closely following the Wav2Vec2 architecture, trained on 53 languages, including Italian.
- [XLSR-128](https://huggingface.co/facebook/wav2vec2-xls-r-300m): a pre-trained model, closely following the Wav2Vec2 architecture, trained on 128 languages, including Italian.
- [ECAPA](https://huggingface.co/speechbrain/lang-id-voxlingua107-ecapa): a model pre-trained for the language identification on VoxLingua107 dataset (including Italian).

