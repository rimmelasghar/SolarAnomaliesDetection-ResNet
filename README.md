# SolarAnomaliesDetection using ResNet 🤖

## Abstract
The rapid industrial growth in solar energy is gaining increasing interest in renewable power from smart grids and plants. Anomaly detection in photovoltaic (PV) systems is a demanding task. In this sense, it is vital to utilize the latest updates in machine learning technology to accurately and timely disclose different system anomalies.

## DataSet Information:
InfraredSolarModules is a machine learning dataset that contains real-world imagery of different anomalies found in solar farms. This dataset can be used for machine learning research to gain efficiencies in the solar industry. Infrared imagery is not widely available to researchers. In order to combat the lack of publicly available data on infrared imagery of anomalies in solar PV, this project presents a novel, labeled dataset to facilitate research to solve problems well suited for machine learning that can have environmental impact.

## Description of the dataset 📝

The dataset consists of 20,000 infrared images that are 24 by 40 pixels each. There are 12 defined classes of solar modules presented in this paper with 11 classes of different anomalies and the remaining class being No-Anomaly (i.e. the null case).

|   Class Name   | Images |                                Description                                |
|:--------------:|:------:|:-------------------------------------------------------------------------:|
| Cell           | 1,877  | Hot spot occurring with square geometry in single cell.                   |
| Cell-Multi     | 1,288  | Hot spots occurring with square geometry in multiple cells.               |
| Cracking       | 941    | Module anomaly caused by cracking on module surface.                      |
| Hot-Spot       | 251    | Hot spot on a thin film module.                                           |
| Hot-Spot-Multi | 247    | Multiple hot spots on a thin film module.                                 |
| Shadowing      | 1056   | Sunlight obstructed by vegetation, man-made structures, or adjacent rows. |
| Diode          | 1,499  | Activated bypass diode, typically 1/3 of module.                          |
| Diode-Multi    | 175    | Multiple activated bypass diodes, typically affecting 2/3 of module.      |
| Vegetation     | 1,639  | Panels blocked by vegetation.                                             |
| Soiling        | 205    | Dirt, dust, or other debris on surface of module.                         |
| Offline-Module | 828    | Entire module is heated.                                                  |
| No-Anomaly     | 10,000 | Nominal solar module.                                                     |

Dataset link: [ Click Here](https://github.com/rimmelasghar/Solar-Anamolies-DataSet)

## 👷 Building the model architecture 👷

We are going to use ResNet, which have been one of the major breakthrough in computer vision since they were introduced in 2015.

In ResNets, unlike in traditional neural networks, each layer feeds into the next layer, we use a network with residual blocks, each layer feeds into the next layer and directly into the layers about 2–3 hops away, to avoid over-fitting (a situation when validation loss stop decreasing at a point and then keeps increasing while training loss still decreases). This also helps in preventing vanishing gradient problem and allow us to train deep neural networks. Here is a simple residual block:
![Untitled](https://github.com/rimmelasghar/SolarAnomaliesDetection-ResNet/assets/82160813/025e6ffe-6712-43c5-a8e4-c2f62618cd9f)

## Anomalies in the DataSet:
This below image shows the dataset images shown in batches.
![image](https://github.com/rimmelasghar/SolarAnomaliesDetection-ResNet/assets/82160813/6da57add-884d-4058-829f-6d5dec3f7fd4)

## Accuracy Score:
getting around 80.2% Accurate Results

# Troubleshooting
If you are facing any problems, feel free to open an issue or contact me on `rimmelasghar4@gmail.com` 


[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
<br>
Developed by Rimmel with ❤️




