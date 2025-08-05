# Dataset Descriptions

## Overview

This document provides comprehensive information about the imbalanced time series datasets used in our TDBCL experiments. All datasets are publicly available from established archives and represent diverse real-world applications where class imbalance is a significant challenge.

## Data Sources

- **UCR Time Series Classification Archive**: https://www.cs.ucr.edu/~eamonn/time_series_data_2018/
- **UEA Multivariate Time Series Classification Archive**: http://www.timeseriesclassification.com/

## Dataset Selection Criteria

- **Univariate (UCR)**: Imbalance ratio ≥ 4.0 in training set
- **Multivariate (UEA)**: Imbalance ratio ≥ 2.0 in training set

## Univariate Time Series Datasets (UCR Archive)

| Dataset                      | IR    | Domain    | Train | Test | Classes | Length | Description |
| ---------------------------- | ----- | --------- | ----- | ---- | ------- | ------ | ----------- |
| ECG5000                      | 146.0 | Medical   | 500   | 4500 | 5       | 140    | Cardiac arrhythmia detection from ECG signals |
| FiftyWords                   | 52.0  | Image     | 450   | 455  | 50      | 270    | Word recognition from character outlines |
| MedicalImages                | 33.8  | Medical   | 381   | 760  | 10      | 99     | Medical image classification |
| WordSynonyms                 | 30.0  | NLP       | 267   | 638  | 25      | 270    | Synonym identification from word outlines |
| Phoneme                      | 24.0  | Speech    | 214   | 1896 | 39      | 1024   | Phoneme recognition from audio signals |
| DistalPhalanxTW              | 11.8  | Medical   | 400   | 139  | 6       | 80     | Age group classification from bone outlines |
| ProximalPhalanxTW            | 11.3  | Medical   | 400   | 205  | 6       | 80     | Age group classification from bone outlines |
| Wafer                        | 9.3   | Industrial| 1000  | 6164 | 2       | 152    | Semiconductor wafer defect detection |
| DistalPhalanxOutlineAgeGroup | 8.6   | Medical   | 400   | 139  | 3       | 80     | Age classification from bone X-rays |
| FacesUCR                     | 8.3   | Image     | 200   | 2050 | 14      | 131    | Face recognition from image outlines |
| PLAID                        | 6.8   | IoT       | 537   | 537  | 11      | 1344   | Appliance identification from power consumption |
| MiddlePhalanxTW              | 6.4   | Medical   | 399   | 154  | 6       | 80     | Age group classification from bone outlines |
| DiatomSizeReduction          | 6.0   | Biology   | 16    | 306  | 4       | 345    | Diatom size classification |
| Mallat                       | 5.5   | Synthetic | 55    | 2345 | 8       | 1024   | Synthetic time series with different dynamics |
| Earthquakes                  | 4.6   | Seismic   | 322   | 139  | 2       | 512    | Earthquake vs. explosion classification |
| Worms                        | 4.5   | Biology   | 181   | 77   | 5       | 900    | Nematode behavior classification |
| MiddlePhalanxOutlineAgeGroup | 4.3   | Medical   | 400   | 154  | 3       | 80     | Age classification from bone X-rays |

## Multivariate Time Series Datasets (UEA Archive)

| Dataset     | IR    | Domain      | Train | Test | Features | Classes | Length | Description |
| ----------- | ----- | ----------- | ----- | ---- | -------- | ------- | ------ | ----------- |
| LSST        | 111.0 | Astronomy   | 2459  | 2466 | 6        | 14      | 36     | Large Synoptic Survey Telescope object classification |
| EigenWorms  | 4.6   | Biology     | 128   | 131  | 6        | 5       | 17984  | C. elegans behavior analysis from movement data |
| Handwriting | 4.0   | Recognition | 150   | 850  | 3        | 26      | 152    | Character recognition from pen movement trajectories |
| Heartbeat   | 2.6   | Medical     | 204   | 205  | 61       | 2       | 405    | Normal vs. abnormal heartbeat classification |

## Key Statistics

- **Few-shot scenarios**: Phoneme (single samples per class), DiatomSizeReduction (16 training samples)
- **Multi-class complexity**: FiftyWords (50 classes), Phoneme (39 classes)
- **High-dimensional multivariate**: Heartbeat (61 features), EigenWorms (17984 length)



## Citation

If you use these datasets in your research, please cite the original UCR/UEA archives:

```bibtex
@article{dau2019ucr,
  title={The UCR time series classification archive},
  author={Dau, Hoang Anh and Keogh, Eamonn and Kamgar, Kaveh and others},
  journal={IEEE/CAA Journal of Automatica Sinica},
  year={2019}
}

@article{uea,
  title={The UEA multivariate time series classification archive, 2018},
  author={Bagnall, Anthony and Dau, Hoang Anh and Lines, Jason and Flynn, Michael and Large, James and Bostrom, Aaron and Southam, Paul and Keogh, Eamonn},
  journal={arXiv preprint arXiv:1811.00075},
  year={2018}
}
```
