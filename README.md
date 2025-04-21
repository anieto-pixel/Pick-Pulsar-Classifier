
# Pick-Pulsar-Classifier

Pulsars are important objects of astronomical study. From our telescopes, they appear as relatively periodical pulses of radiation bursts. Due to various factors, such as how weak the signals usually are, and how artificial signals may interfere with them, pulsar detection is often difficult and time-consuming for astronomers. Most pulsar candidates examined by astronomers turn out to not be pulsars, which leads to wasted time and money for research efforts.

Learning algorithms may offer a way to speed this process and reduce the amount of human labor required. Supervised learning algorithms are a subcategory of machine learning defined by the use of labeled data to train a classifier model. Input data is fed to the model, consisting of a set of parameters (or attributes) and a label. The algorithm adjusts the weights attributed to each parameter until the model is appropriately fit. This model can then be used to classify objects in new datasets.

Astronomy has collected various unbalanced datasets of pulsar candidates that have already been classified by human astronomers. This study aims to assess whether supervised learning models trained on these datasets can be effective enough at classifying previously unseen objects as either pulsars or non-pulsars to aid astronomical research.

This project evaluates the performance of different classifiers when trained on balanced datasets created using various sampling techniques. It then compares how each classifier performs when classifying both balanced and unbalanced test sets. The goal is to support human-in-the-loop systems by minimizing false negatives—ensuring that true pulsars are not missed.

---

# 📁 Project Structure

```bash
Pick-Pulsar-Classifier/
│
├── data/
│   └── HTRU_2.csv                   # Dataset of pulsar candidates
│
├── notebooks/
│   ├── 01_data_visualization.ipynb        # Exploratory data analysis
│   ├── 02_aux_methods.ipynb               # Helper methods and utilities
│   ├── 03_sampling_and_comparison.ipynb   # Sampling techniques + classifier evaluation
│   └── 04_classifier_tester.ipynb         # Final comparative testing
│
├── requirements.txt               # Dependencies for the project
└── README.md                      # Project description and setup


# Settup Instructions

git clone https://github.com/anieto-pixel/Pick-Pulsar-Classifier.git
cd Pick-Pulsar-Classifier

python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate

conda create -n pulsar-classifier python=3.10
conda activate pulsar-classifier

pip install -r requirements.txt
pip install pandas numpy matplotlib scikit-learn imbalanced-learn
