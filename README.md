# SALVI: Speech Analysis of Language Varieties in Italy

This repository contains the information and the code for the SALVI project, aiming at analyzing Italian language varieties from a speech perspective. You can freely access the full paper [here](https://aclanthology.org/2024.lrec-main.1317/).

**Code and additional details for data downloading and splitting will be available soon**.

## Data

The main dataset currently used for the project is the [VIVALDI](https://www2.hu-berlin.de/vivaldi/) and its development is out of the scope for this project.

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

## Referencing

Below is the citation for our paper presented at LREC-COLING 2024.

```bibtex
@inproceedings{la-quatra-etal-2024-speech-analysis,
    title = "Speech Analysis of Language Varieties in {I}taly",
    author = "La Quatra, Moreno  and
      Koudounas, Alkis  and
      Baralis, Elena  and
      Siniscalchi, Sabato Marco",
    editor = "Calzolari, Nicoletta  and
      Kan, Min-Yen  and
      Hoste, Veronique  and
      Lenci, Alessandro  and
      Sakti, Sakriani  and
      Xue, Nianwen",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italy",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.1317",
    pages = "15147--15159",
}
```
