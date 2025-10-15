## Conference
This work is part pf my paper **Communication-Efficient Federated Learning via Adaptive Single-Layer Transmission** submitted to **The 8th International Conference on Advanced Communication Technologies and Networking (CommNet 2025)**.

## Credits
**Author:** Khaji Sana 
**Supervised by:** Yann BEN MAISSA (INPT)
The National Institute of Posts and Telecommunications(INPT)

## Description
This implementation presents an eXtreme Federated Learning approach guided by Sensitivity (XFL-S) that uses sensitivity-based layer selection to reduce communication overhead. 

## Installation

\`\`\`bash
pip install -r requirements.txt
\`\`\`

Or install manually:
\`\`\`bash
pip install flwr[simulation] flwr-datasets[vision] torch torchvision numpy scikit-learn
\`\`\`

## How to Run

### Running the Jupyter Notebook

1. Install Jupyter:
\`\`\`bash
pip install jupyter
\`\`\`

2. Launch Jupyter:
\`\`\`bash
jupyter notebook
\`\`\`

3. Open `xfl_s_main.ipynb` in your browser

4. Select your scenario in the configuration cell (Cell 4):
\`\`\`python
# Uncomment ONE scenario:
# scenario_config = SCENARIOS["6_layer_iid"]
# scenario_config = SCENARIOS["6_layer_noniid"]
# scenario_config = SCENARIOS["10_layer_iid"]
scenario_config = SCENARIOS["10_layer_noniid"]
\`\`\`

5. Run all cells (Cell > Run All)

## Experimental Scenarios

| Scenario | Model | Data Distribution | Clients | Epochs |
|----------|-------|-------------------|---------|--------|
| 6_layer_iid | 6 layers | IID | 18 | 40 |
| 6_layer_noniid | 6 layers | Non-IID | 30 | 50 |
| 10_layer_iid | 10 layers | IID | 18 | 40 |
| 10_layer_noniid | 10 layers | Non-IID | 30 | 50 |

## Project Files
\`\`\`
├── README.md
├── xfl_s_main.ipynb         # Main notebook
├── requirements.txt
\`\`\`

## Citation
\`\`\`
This work is inspired by:
R. El Mokadem, Y. Ben Maissa, and Z. El Akkaoui,
“Extreme Federated Learning (XFL): A Layer-Wise Approach,”
Cluster Computing, 2024
