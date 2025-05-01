# GA_WarmStart
A hybrid approach to warm-start Genetic Algorithms using neural network predictions. The model forecasts individual survival and guides initial population selection, improving convergence and optimization performance. Includes baseline comparison, visualizations, and evaluation metrics.


Key Features
  1. Neural network predicts individual survival from GA history.
  2. Warm-start GA using a mix of top-k and mid-k predicted individuals.
  3. Baseline GA and warm-start GA performance comparison.
  4. Visualizations of convergence and evaluation metrics.




Repository Structure
GA_MCS_v4.ipynb – Complete pipeline: simulation, model training, and warm-started GA experiments.


Requirements
Install dependencies using pip:

pip install torch scikit-learn numpy pandas matplotlib tqdm
You’ll also need Python 3.7+.

Running the Notebook
Clone the repository:


git clone https://github.com/aniketbhaumik/warm-start-ga.git
cd warm-start-ga
Open the Jupyter Notebook:


jupyter notebook GA_MCS_v4.ipynb
Run the notebook cell by cell to:

  1. Generate simulated optimization data
  2. Train the neural network to predict GA survival
  3. Warm-start the GA with predicted top-k/mid-k individuals
  4. Compare baseline vs. warm-started GA runs

Reproducibility Notes:
GA population is randomly initialized; set random seeds for deterministic runs.

Hyperparameters (e.g., population size, selection ratio) can be tuned in notebook cells.

Ablation studies for different sequence lengths and top-k configurations included.

License:
This project is licensed under the MIT License. You are free to use, modify, and distribute this code with attribution.

Acknowledgments:
Created as part of a research project in genetic algorithm optimization using machine learning. Reach out for collaborations or questions!
