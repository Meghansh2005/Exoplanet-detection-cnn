# 🚀 Project Stargazer: Anomaly Detection in the Kepler Sector

## 🌌 MISSION LOG

**Objective:** To sift through the cosmic noise and identify the faint shadows of distant worlds. Our primary instrument is a deep learning neural core, tasked with analyzing stellar light-flux transmissions from the NASA Kepler deep-space telescope.

The mission is to detect anomalies—the minute, periodic dips in starlight that betray the presence of a transiting exoplanet. We are hunting for new worlds, one star at a time.

This is a high-stakes search. The signals are faint, and true targets are needles in a cosmic haystack. Our AI must learn to distinguish the whisper of a planet from the roar of a star.



---

## 🛰️ DATASET: Stellar Transmissions

The mission data was acquired from the Kepler Telescope archives. Due to the large size of the transmission logs, they are not stored in this repository.

* **You can download the dataset directly from Kaggle:**
    [**Exoplanet Hunting in Deep Space Dataset**](https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data)

You will need to download `exoTrain.csv` and `exoTest.csv` and place them in the main project folder.

---

## 📡 SIGNAL PROCESSING & NEURAL ARCHITECTURE

Our neural core, codenamed **"Pathfinder"**, follows a strict protocol to calibrate and analyze incoming stellar data.

1.  **Acquiring Transmissions**: Raw data packets from `exoTrain.csv` and `exoTest.csv` are interfaced with the system.
2.  **Signal Calibration**: Each raw signal is unstable. Pathfinder normalizes the transmission, centering the flux signal to a mean of 0 and scaling its variance to 1.
3.  **Signal Enhancement**: To amplify the faint signature of a potential transit, a secondary "smoothing" channel is synthesized via a uniform filter.
4.  **The Neural Core**: A 1D Convolutional Neural Network with multiple layers of cognitive filters (`Conv1D`), pattern sub-sampling (`MaxPool1D`), and synaptic stabilization (`BatchNormalization`).
5.  **Cognitive Training Protocols**:
    * **Balanced Reality Simulator**: A custom data generator creates balanced training batches to overcome the rarity of positive signals.
    * **Temporal Augmentation**: The simulator randomly shifts signals in time to make the model more robust.
    * **Adaptive Learning Modulator (`ReduceLROnPlateau`)**: An automated scheduler dynamically adjusts the core's learning rate for optimal performance.

---

## 🎯 MISSION FINDINGS

**System Performance: Target Lock Confirmed.**

Pathfinder has achieved **near-perfect target discrimination**, successfully identifying planetary signatures with extremely high accuracy. The deployed confusion matrix provides a full diagnostic breakdown of its classification performance.

---

## ⚙️ ENGAGING THE SYSTEM

To replicate this mission on your local starship's computer:

1.  **Clone the Mission Code:**
    ```bash
    git clone [https://github.com/YourUsername/Exoplanet-detection-cnn.git](https://github.com/YourUsername/Exoplanet-detection-cnn.git)
    cd Exoplanet-detection-cnn
    ```
2.  **Acquire the Data:** Download the `exoTrain.csv` and `exoTest.csv` files from the [Kaggle link](https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data) and place them in the cloned folder.
3.  **Install Required Technologies:**
    Engage a virtual environment for optimal performance.
    ```bash
    pip install -r requirements.txt
    ```
4.  **Initiate Analysis:**
    Launch the Jupyter interface and open the mission file: `exoplanet_detection_cnn.ipynb`.
    ```bash
    jupyter notebook
    ```
