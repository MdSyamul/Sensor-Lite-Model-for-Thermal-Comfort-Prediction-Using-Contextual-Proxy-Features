# Sensor-Lite Model for Thermal Comfort Prediction Using Contextual Proxy Features

## Overview

This repository provides code and resources for the paper **"Sensor-Lite Model for Thermal Comfort Prediction Using Contextual Proxy Features"**. The main objective is to accurately predict thermal comfort levels in indoor environments using minimal sensor data, leveraging contextual proxy features to maintain prediction accuracy with reduced hardware requirements.

## Table of Contents

- [Introduction](#introduction)
- [Key Features](#key-features)
- [Getting Started](#getting-started)
- [Requirements](#requirements)
- [Usage](#usage)
- [Data](#data)
- [Model Description](#model-description)
- [Results](#results)
- [Citation](#citation)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Introduction

Thermal comfort is a crucial factor in building environments, affecting both occupant well-being and energy efficiency. Traditional models rely on extensive sensor data, which can be costly and difficult to maintain. This project proposes a sensor-lite approach by substituting some physical sensor inputs with contextual proxy features (such as occupancy, time, and weather data), reducing hardware needs without sacrificing prediction performance.

## Key Features

- Predicts thermal comfort using reduced sensor input.
- Utilizes contextual proxy features to enhance model accuracy.
- Includes code for data preprocessing, model training, and evaluation.
- Modular design for easy adaptation to other comfort metrics or buildings.

## Getting Started

Clone the repository:

```bash
git clone https://github.com/MdSyamul/Sensor-Lite-Model-for-Thermal-Comfort-Prediction-Using-Contextual-Proxy-Features.git
cd Sensor-Lite-Model-for-Thermal-Comfort-Prediction-Using-Contextual-Proxy-Features
```

## Requirements

- Python 3.7+
- pandas
- numpy
- scikit-learn
- matplotlib

Install dependencies with:

```bash
pip install -r requirements.txt
```

## Usage

1. Place your dataset in the `data/` directory.
2. Modify configuration parameters in `config.py` as needed.
3. Run the main script to preprocess data, train, and evaluate the model:

```bash
python main.py
```

4. Results and output files will be saved in the `results/` directory.

## Data

Sample and/or preprocessed datasets are provided in the `data/` directory. The dataset typically includes:

- Environmental sensor readings (temperature, humidity, etc.)
- Contextual proxy features (occupancy, time, external weather)
- Occupant feedback (thermal comfort votes)

**Note:** For privacy or licensing reasons, you may need to request access or use your own dataset.

## Model Description

The model leverages machine learning techniques (such as Random Forests, XGBoost, or neural networks) to predict thermal comfort labels. The key innovation is the use of contextual proxy features to replace certain sensor inputs (e.g., replacing direct CO2 measurements with occupancy patterns).

### Steps:

1. **Data Preprocessing:** Cleans and formats sensor and contextual data.
2. **Feature Selection:** Identifies essential proxy features.
3. **Model Training:** Fits selected ML models.
4. **Evaluation:** Compares sensor-lite vs. full-sensor model performance.

## Results

The sensor-lite model achieves comparable accuracy to full-sensor models, demonstrating the effectiveness of contextual proxy features. Detailed results, plots, and analysis can be found in the `results/` directory and the accompanying paper.

## Citation

If you use this code or data in your research, please cite.

## Acknowledgements

We thank the data providers and open-source community.

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for details.
