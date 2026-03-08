# Wild Animal Detection from Animal Sound

This project develops a deep learning system that identifies wild animals based on their vocal sounds.  
The model analyzes audio recordings and classifies the animal species using Convolutional Neural Networks (CNN).

The system is designed to support wildlife monitoring, conservation research, and early detection of animal presence in human–wildlife conflict zones.

---

## Animals Detected
The model classifies sounds from six animal species:

- Bat
- Chimpanzee
- Elephant
- Frog
- Horse
- Tiger

---

## Technologies Used

- Python
- TensorFlow / Keras
- Librosa
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

---

## Methodology

1. **Data Collection**
   - Animal sound recordings collected from online sources.
   - Dataset contains **660 audio clips** across 6 classes.

2. **Preprocessing**
   - Audio files converted to `.wav`
   - Noise removal and normalization.

3. **Feature Extraction**
   - MFCC (Mel-Frequency Cepstral Coefficients)
   - Delta MFCC
   - Delta-Delta MFCC

4. **Data Augmentation**
   - Noise injection
   - Time shifting

5. **Model Training**
   - CNN models tested (Adam, Nadam, Adagrad)
   - Final model: **LeNet-based CNN**

---

## Model Performance

| Model | Test Accuracy |
|------|------|
| CNN (Adagrad) | 94.81% |
| CNN (Adam) | 94.07% |
| CNN (Nadam) | 93.33% |
| ResNet | 91.11% |
| DenseNet | 91.11% |
| **LeNet CNN (Final Model)** | **99.50%** |

---

## Workflow

Audio Input  
→ Feature Extraction (MFCC)  
→ Data Preprocessing  
→ CNN Model Training  
→ Animal Sound Classification

---

## Results

- Training Accuracy: **100%**
- Testing Accuracy: **99.5%**
- High precision and recall across all animal classes.

The model was also tested on **external audio samples** and successfully classified them, demonstrating strong generalization ability.

---

## Applications

- Wildlife monitoring
- Animal conservation research
- Bioacoustics analysis
- Early warning systems for human–wildlife conflict

---

## Future Improvements

- Expand dataset with more species
- Real-time sound detection system
- Deploy model on edge devices for field monitoring

---

## Author

Teneti Srujana  
Artificial Intelligence & Data Science  
CBIT, Hyderabad
