# Sensor-Lite Model for Thermal Comfort Prediction Using Contextual Proxy Features

## Overview

The Predicted Mean Vote (PMV) is a widely used measure of thermal comfort. It needs six inputs, including mean radiant temperature. Measuring mean radiant temperature (MRT) often needs sensors like black globe thermometers, which are slow to respond and difficult to set up. Existing AC or HVAC systems rarely include these sensors, and adding them increases cost. This makes it harder for current AC systems to scale for monitoring occupants’ comfort and autonomously adjust to a target comfort level (e.g., a PMV of 0). This study estimates PMV without directly measuring MRT by using easily available context variables that reflect radiative conditions, such as season, building type, monthly outdoor air temperature, and climate. From the ASHRAE Thermal Comfort Database II, we selected nine features: five standard inputs (air temperature, air velocity, relative humidity, metabolic rate, and clothing insulation) and four contextual proxies for MRT (season, building type, monthly outdoor air temperature, and climate). Three machine learning models—Deep Neural Networks, Gradient Boosting Regression, and Random Forest—were developed to estimate PMV. Among the models, the DNN performed best, with an MSE of 0.01865, MAE of 0.08821, and R² of 0.96681. This shows that MRT can be effectively replaced with proxy variables such as season, climate, building type, and monthly outdoor temperature while still achieving high prediction accuracy. These results suggest that existing AC/ HVAC systems do not need additional radiant temperature sensors to monitor and maintain a target thermal comfort level.

## Table of Contents

- [Getting Started](#getting-started)
- [Requirements](#requirements)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Getting Started

Clone the repository:

```bash
git clone https://github.com/MdSyamul/Sensor-Lite-Model-for-Thermal-Comfort-Prediction-Using-Contextual-Proxy-Features.git
cd Sensor-Lite-Model-for-Thermal-Comfort-Prediction-Using-Contextual-Proxy-Features
```

## Requirements

- Python 3.10

Install dependencies with:

```bash
pip install -r requirements.txt
```


## Acknowledgements

We thank the data providers and open-source community.

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for details.
