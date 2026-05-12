# EuroSAT Satellite Image Classification

This project demonstrates the classification of satellite images from the EuroSAT dataset using deep learning and transfer learning techniques.

The model classifies satellite images into 10 land-cover categories:

- Forest
- River
- Residential
- Industrial
- Highway
- SeaLake
- Pasture
- AnnualCrop
- PermanentCrop
- HerbaceousVegetation

The project is implemented using TensorFlow/Keras and can be run in a local environment or cloud platforms like Google Colab.

---

## Dataset

**Dataset:** EuroSAT Dataset

**Source:** [EuroSAT Dataset on Kaggle](https://www.kaggle.com/datasets/apollo2506/eurosat-dataset)

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Pandas
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Model Architecture

The project employs transfer learning with MobileNetV2, pre-trained on ImageNet.

**Architecture:**

- MobileNetV2 base model (with frozen layers)
- Global Average Pooling 2D
- Dense layer (128 units, ReLU activation)
- Dropout layer (for regularization)
- Output layer (10 units, Softmax activation)

**Techniques Applied:**

- Data augmentation (rotation, shifting, zooming, flipping)
- Transfer learning
- Fine-tuning
- Early stopping

---

## Results

- Achieved approximately 90% validation accuracy (results may vary based on training)
- Effective reduction of overfitting through data augmentation and dropout
- Successful classification of satellite images into all 10 categories

---

## Repository Structure

```
satellite-image-classification/
│
├── data/
│   └── EuroSAT/          # Dataset directory
├── ml_env/               # Virtual environment
├── model/                # Saved models
├── notebooks/
│   └── EuroSAT_Project.ipynb  # Main notebook
├── README.md
├── SOLUTION.md
└── .gitignore
```

---

## Setup and Usage

1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt` (if available).
3. Activate the virtual environment: `ml_env\Scripts\activate` (Windows).
4. Open the notebook: `jupyter notebook notebooks/EuroSAT_Project.ipynb`.
5. Run the cells to train the model or make predictions.

---

## Future Improvements

- Deploy the model using Streamlit for a web interface
- Perform hyperparameter tuning for better performance
- Experiment with other architectures like ResNet or EfficientNet
- Implement real-time satellite image analysis
- Add more evaluation metrics and visualizations

---

## Recommendations

- Keep large datasets and trained model files out of version control using `.gitignore`.
- Use a dependency lock file such as `requirements.txt` to ensure reproducible environments.
- Prefer storing raw data outside the repository or using a script to download it on demand.
- Save generated plots and checkpoints to `images/` and `model/`, but do not commit them.
- Document the exact training and evaluation workflow in the notebook or README.

---

## Author

Sammy Atale

**Interests:**

- Machine Learning
- Artificial Intelligence
- Computer Vision
* Space Technologies
