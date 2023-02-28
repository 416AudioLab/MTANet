# MMNet

## Introduction

The official implementation of "MMNET: Multi-band Time-frequency attention Network (MTANet) for Singing Melody Extraction from Polyphonic Music, whose manuscript is under submission for interspeech 2023.

We propose a more powerful singing melody extractor named multi-band multi-scale network (MMNet) for polyphonic music. Experimental results show that our proposed MMNet achieves promising performance compared with existing state-of-the-art methods, while keeping with a small number of network parameters.

<p align="center">
<img src="fig/arch.png" align="center" alt="MMNet Architecture" width="100%"/>
</p>

## Getting Started

### Download Datasets

* [MIR-1k](https://sites.google.com/site/unvoicedsoundseparation/mir-1k)
* [ADC 2004 & MIREX05](https://labrosa.ee.columbia.edu/projects/melody/)
* [MedleyDB](https://medleydb.weebly.com/)

After downloading the data, use the txt files in the data folder, and process the CFP feature by [feature_extraction.py](feature_extraction.py).

## Model implementation

Refer to the file: [mmnet.py](model/mmnet.py)

## Result

### Prediction result

The visualization illustrates that our proposed MMNet can avoid the octave errors and reduce the melody detection errors.

<p align="center">
<img src="fig/estimation.png" align="center" alt="Estimation" width="60%"/>
</p>

### Comprehensive result

The scores here are either taken from their respective papers or from the result implemented by us. Experimental results show that our proposed MMNet achieves promising performance compared with existing state-of-the-art methods.

<p align="center">
<img src="fig/result.png" align="center" alt="Result" width="50%"/>
</p>

### Ablation study result

we conducted seven ablations to verify the effectiveness of each design in the proposed network. Due to the page limit, we selected the ADC2004 dataset for ablation study in the paper. More detailed results are presented here.

<p align="center">
<img src="fig/ablution_ADC2004.png" align="center" alt="ablution_ADC2004" width="50%"/>
</p>

<p align="center">
<img src="fig/ablution_MIREX 05.png" align="center" alt="ablution_MIREX 05" width="50%"/>
</p>

<p align="center">
<img src="fig/ablution_MEDLEY DB.png" align="center" alt="ablution_MEDLEY DB" width="50%"/>
</p>

## Download the pre-trained model

Refer to the file: [pre-train model](pre-train model/)
