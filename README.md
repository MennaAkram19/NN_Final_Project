# 👩‍💻 Neural Network (MLP) Project

## 👤 Name: Menna Akram Mahmoud

## 📌 Project Idea
In this project, I built a Multilayer Perceptron (MLP) model using PyTorch for image classification. The main goal was to classify clothing images from the Fashion-MNIST dataset into their correct categories. I also experimented with different model architectures and learning rates to compare the performance of each experiment.

---

## 📊 Dataset

## Dataset Details
- 60,000 training images
- 10,000 testing images
- 10 output classes
- Image size: 28 × 28

## Dataset Split
- Training set
- Validation set
- Test set

The dataset was loaded using torchvision and divided into training, validation, and testing sets.

---

## ⚙️ Data Preprocessing

## Preprocessing Steps
- Converting images into tensors
- Normalizing pixel values
- Splitting the training data into training and validation sets using an 80/20 ratio

These preprocessing steps helped improve model performance and training stability.

---

## 🧠 Model Architecture

## ✅ Experiment 1

## Model Structure
- Flatten input layer
- Two hidden layers:
  - 256 neurons
  - 128 neurons
- ReLU activation function
- Batch Normalization
- Dropout (0.3)
- Output layer with 10 neurons

## Learning Rate

```python
0.001
```

---

## ✅ Experiment 2

## Model Structure
- Flatten layer
- Three hidden layers:
  - 512 neurons
  - 256 neurons
  - 128 neurons
- ReLU activation
- Batch Normalization
- Dropout layers
- Output layer with 10 classes

## Learning Rate

```python
0.0001
```

---

## 🏋️ Training Process

## Training Configuration
- Adam optimizer
- CrossEntropyLoss
- Batch size = 64
- 10 epochs

## Monitored Metrics
- Training Loss
- Validation Loss
- Training Accuracy
- Validation Accuracy

These metrics helped evaluate model performance and detect overfitting during training.

---

## 🔬 Experiments Comparison

## Comparison Between Experiment 1 and Experiment 2

| Feature | Experiment 1 | Experiment 2 |
|---|---|---|
| Hidden Layers | 2 Hidden Layers | 3 Hidden Layers |
| Neurons | 256 → 128 | 512 → 256 → 128 |
| Learning Rate | 0.001 | 0.0001 |
| Dropout | 0.3 | 0.3 / 0.2 |
| Batch Normalization | Yes | Yes |
| Optimizer | Adam | Adam |
| Loss Function | CrossEntropyLoss | CrossEntropyLoss |
| Epochs | 10 | 10 |
| Batch Size | 64 | 64 |
| Accuracy | ~88% | ~89% |
| Generalization | Good | Better |
| Training Stability | Stable | More Stable |

---

## 📌 Comparison Conclusion

Experiment 1 achieved good performance with a simpler architecture and faster learning rate.

Experiment 2 achieved slightly better accuracy and generalization because the deeper architecture was able to learn more complex patterns from the dataset. The smaller learning rate also helped make training more stable and reduced fluctuations during optimization.

---

## 📈 Results

## Final Accuracy

```python
88% – 89%
```

The deeper model showed better generalization and more stable validation performance.

---

## 📊 Visualizations

## Generated Plots
- Training vs Validation Loss
- Training vs Validation Accuracy
- Comparison between both experiments

These visualizations helped analyze the model behavior during training.

---

## 🧪 Regularization Techniques

## Techniques Used
- Dropout
- Batch Normalization

These techniques helped reduce overfitting and improve generalization.

---

## 🚀 Running the Project

## Install Required Libraries

```bash
pip install torch torchvision matplotlib pandas
```

---

## 📌 Final Notes

This project was implemented using PyTorch and follows a complete deep learning workflow including:
- data preprocessing
- model building
- training
- validation
- testing
- performance visualization

The experiments helped in understanding how different hyperparameters affect neural network performance.
