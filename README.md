[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.nm000262-blue)](https://doi.org/10.82901/nemar.nm000262)

# P300 BCI EEG dataset (Chailloux Peguero et al. 2020)

## Overview

A P300 brain-computer interface dataset comprising EEG recordings from 19 healthy participants across 3 sessions each. The study investigates how visual stimulation conditions (standard flash vs. cartoon face stimuli) affect P300-BCI performance using an 8-channel montage sampled at 256 Hz. Data were collected using a P300 paradigm with 5 grid sizes (4-9 symbols) and include target and non-target event classifications.

## Dataset Summary

| Property | Value |
|---|---|
| Subjects | 19 |
| Channels | 8 |
| Classes | 2 |
| Trial length | 1 s |
| Sampling frequency | 256 Hz |
| Sessions | 3 |

| Paradigm | P300 |

## Data Collection Methods

EEG data were acquired using a g.USBamp amplifier (g.tec) with 8 passive g.SCARABEO electrodes positioned at Fz, Cz, P3, Pz, P4, PO7, PO8, and Oz according to the standard 10-20 montage. Sampling rate was 256 Hz with right earlobe reference and AFz ground. Line frequency was 60 Hz. The P300 paradigm employed visual stimulation with two stimulus types (standard flash and cartoon face) across 5 grid sizes (4-9 symbols), with an inter-stimulus interval of 75 ms and stimulus onset asynchrony of 150 ms.

## How to Access via MOABB

Install MOABB and load this dataset directly:

```python
from moabb.datasets import Chailloux2020
from moabb.paradigms import P300
paradigm = P300()

dataset = Chailloux2020()
X, y, metadata = paradigm.get_data(dataset)
```

For more details see the [MOABB documentation](https://moabb.neurotechx.com/) and the
[MOABB dataset page](https://moabb.neurotechx.com/docs/generated/moabb.datasets.Chailloux2020.html).

## Citation

If you use this dataset please cite the primary publication:

> DOI: [10.3390/s20247198](https://doi.org/10.3390/s20247198)

## NEMAR / MOABB Benchmark Collection

This BIDS-formatted dataset was converted from the original data using the
[MOABB](https://moabb.neurotechx.com/) pipeline and re-hosted on
[NEMAR](https://nemar.org/) as part of the MOABB benchmark collection.
The original data and license terms apply — see `dataset_description.json` for details.
