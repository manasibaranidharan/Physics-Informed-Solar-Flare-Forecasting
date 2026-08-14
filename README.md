# Physics-Informed-Solar-Flare-Forecasting

### Physics-Informed Neural Network for Explainable Solar Flare Nowcasting and Forecasting Using SoLEXS and HEL1OS Data from Aditya-L1

This repository contains the research and implementation of a **Physics-Informed Neural Network (PINN)** framework for solar flare nowcasting and forecasting using X-ray observations from India's **Aditya-L1 mission**.

The proposed system combines **soft X-ray observations from SoLEXS** and **hard X-ray observations from HEL1OS** with physics-informed deep learning and explainable AI techniques to produce more accurate, reliable, and interpretable solar flare predictions.

---

## Overview

Solar flares are powerful bursts of energy from the Sun that can affect technological infrastructure on Earth, including satellite communications, power grids, and aviation systems.

Traditional statistical and machine learning approaches can struggle with:

* Complex solar activity patterns
* High false-alarm rates
* Limited physical interpretability
* Lack of transparency in predictions

This research proposes a **Physics-Informed Neural Network (PINN)** approach that incorporates physical knowledge into the learning process while using multimodal X-ray observations from Aditya-L1.

The system is designed to predict:

* Solar flare occurrence
* Flare intensity
* Flare timing
* Flare class (C, M, and X)

Explainable AI techniques are incorporated to make the predictions more transparent and understandable.

---

## Key Features

* **Physics-Informed Neural Network (PINN)**
* **Multimodal X-ray data integration**
* **SoLEXS soft X-ray observations**
* **HEL1OS hard X-ray observations**
* **Solar flare classification**
* **Explainable AI (XAI)**
* **SHAP-based prediction explanations**
* **Physics-constrained learning**
* **Real-time monitoring concept**
* **Solar flare alerting and decision support**
* **Continuous model improvement**

The methodology combines data-driven learning with physical constraints to improve prediction reliability and reduce false alarms.

---

## Data Sources

The research uses X-ray observations from two instruments aboard the **Aditya-L1 spacecraft**:

### SoLEXS

**Solar Low Energy X-ray Spectrometer (SoLEXS)** provides soft X-ray observations associated with solar activity and flare precursors.

### HEL1OS

**High Energy L1 Orbiting X-ray Spectrometer (HEL1OS)** provides hard X-ray observations that provide information about flare intensity and dynamics.

The combination of soft and hard X-ray information enables multimodal analysis of solar activity.

---

## Methodology

The proposed framework follows the following pipeline:

```text
Aditya-L1 X-ray Data
        │
        ├── SoLEXS
        │     └── Soft X-ray Data
        │
        └── HEL1OS
              └── Hard X-ray Data
                    │
                    ▼
             Data Preprocessing
                    │
                    ▼
             Feature Engineering
                    │
                    ▼
          Multimodal Data Fusion
                    │
                    ▼
       Physics-Informed Neural Network
                    │
             ┌──────┴──────┐
             │             │
      Physics Constraints  Data Learning
             │             │
             └──────┬──────┘
                    ▼
             Flare Prediction
                    │
                    ▼
              XAI / SHAP
                    │
                    ▼
        Explainable Prediction
                    │
                    ▼
          Monitoring & Alerts
```

The methodology includes data collection, preprocessing, feature engineering, physics-informed learning, XAI, model training, validation, multimodal data handling, and a real-time monitoring interface.

---

## Physics-Informed Learning

Unlike a purely data-driven neural network, the proposed PINN incorporates physical knowledge into the training process.

The model learns from historical X-ray observations while simultaneously being guided by physical constraints associated with solar flare activity.

This helps the model produce predictions that are not only data-driven but also consistent with the underlying physical principles of solar activity.

---

## Explainable AI

To improve transparency, the framework incorporates **Explainable AI (XAI)** techniques.

In particular, **SHAP (SHapley Additive exPlanations)** is used to provide interpretable explanations of model predictions.

This allows users to investigate which input features contributed to a predicted solar flare and helps improve trust in automated space-weather forecasting systems.

---

## Results

The research reports the following experimental results:

| Metric                        |         Result |
| ----------------------------- | -------------: |
| Flare classification accuracy |        **95%** |
| Average prediction lead time  | **30 minutes** |
| False-alarm reduction         |        **40%** |
| Flare classes                 |    **C, M, X** |

The reported results indicate that the proposed PINN-based approach can provide accurate and interpretable solar flare predictions while reducing false alarms.

---

## Evaluation Metrics

The model is evaluated using standard machine-learning classification metrics:

* Accuracy
* Precision
* Recall
* F1-score

Additional domain-specific evaluation criteria can be used to assess the effectiveness of solar flare forecasting.

---

## Real-Time Monitoring

The proposed system includes an interactive monitoring concept designed to support space-weather forecasting.

The dashboard can provide:

* Current solar activity
* Predicted flare probability
* Predicted flare class
* Prediction lead time
* Model confidence
* Explainable AI results
* Solar flare alerts

The research proposes an AI decision-support interface for real-time monitoring and timely responses to potential solar flare events.

---

## Technologies

The implementation is based on machine learning, scientific computing, and explainable AI technologies.

Potential components include:

* Python
* PyTorch / TensorFlow
* NumPy
* Pandas
* SciPy
* Matplotlib
* SHAP
* Jupyter Notebook
* Solar X-ray datasets

> The exact implementation stack may evolve as the research implementation progresses.

---

## Project Structure

```text
Physics-Informed-Solar-Flare-Forecasting/
│
├── data/
│   ├── raw/
│   │   ├── solexs/
│   │   └── helios/
│   └── processed/
│
├── notebooks/
│   ├── data_exploration.ipynb
│   ├── preprocessing.ipynb
│   └── model_analysis.ipynb
│
├── src/
│   ├── data/
│   ├── preprocessing/
│   ├── features/
│   ├── models/
│   ├── physics/
│   ├── explainability/
│   └── evaluation/
│
├── dashboard/
│
├── results/
│   ├── figures/
│   └── metrics/
│
├── paper/
│   └── research-paper.pdf
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Research Pipeline

```text
Data Collection
      ↓
Data Cleaning & Preprocessing
      ↓
Feature Engineering
      ↓
SoLEXS + HEL1OS Integration
      ↓
Physics-Informed Model
      ↓
Model Training
      ↓
Validation & Evaluation
      ↓
SHAP Explainability
      ↓
Flare Prediction
      ↓
Monitoring & Alert Generation
```

---

## Research Objectives

The primary objectives of this research are to:

1. Develop a Physics-Informed Neural Network for solar flare forecasting.
2. Integrate soft and hard X-ray observations from Aditya-L1.
3. Improve solar flare classification accuracy.
4. Reduce false alarms through physics-informed learning.
5. Provide explainable predictions using XAI.
6. Provide useful lead time for potential flare events.
7. Develop a framework suitable for space-weather monitoring.

---

## Future Work

Future development can focus on:

* Expanding the available Aditya-L1 dataset
* Improving model accuracy and generalization
* Incorporating additional solar observations
* Improving multimodal fusion
* Developing more advanced physics constraints
* Improving uncertainty estimation
* Deploying the model for real-time forecasting
* Extending the framework to other space-weather phenomena

The paper identifies expanded data sources, improved accuracy, and applications to other space-weather phenomena as potential directions for future research.

---

## Research Paper

**Title:**
*Physics-Informed Neural Network for Explainable Solar Flare Nowcasting and Forecasting Using SoLEXS and HEL1OS Data from Aditya-L1*

**Author:**
**Manasi Baranidharan**

**Institution:**
SRM Institute of Science and Technology, Ramapuram

---

## References

1. Indian Space Research Organisation (ISRO), **Aditya-L1 Mission**.
2. *Physics-Informed Neural Networks for Solar Flare Prediction*, Journal of Space Weather and Space Climate, 2022.
3. *Explainable AI in Space Weather Forecasting: A Case Study on Solar Flares*, IEEE Transactions on Aerospace and Electronic Systems, 2021.
4. *Deep Learning for Solar Flare Prediction Using X-ray Data*, Neural Networks, 2020.
5. *Machine Learning Approaches for Solar Flare Forecasting*, Space Weather, 2020.
6. *Solar Flare Prediction Using Machine Learning and X-ray Observations*, The Astrophysical Journal, 2020.

---

## Author

**Manasi Baranidharan**
B.Sc. Artificial Intelligence and Machine Learning
SRM Institute of Science and Technology, Ramapuram

---

## Acknowledgments

This research acknowledges the open-source research community and the publicly available datasets, tools, libraries, and frameworks that supported the research and experimentation.

---

> **Note:** This repository is intended for research and educational purposes. The reported experimental results correspond to the research paper and should be independently reproduced and validated before use in operational space-weather forecasting.
