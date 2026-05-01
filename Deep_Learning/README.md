# Deep Learning Experiments

A collection of deep learning experiments using TensorFlow/Keras and PyTorch on classic datasets (MNIST, CIFAR-10).

## 📁 Experiments Overview

| File | Description |
|------|-------------|
| `Loading_MNIST_Dataset.ipynb` | Loading and exploring the MNIST dataset |
| `Exp_1.ipynb` | ANN with 10 layers on MNIST — comparing Adam vs SGD optimizers |
| `Exp_2.ipynb` | Further ANN experiments on MNIST |
| `Exp_3.ipynb` | CNN on MNIST with learning rate decay (ReduceLROnPlateau) |
| `Exp_4.ipynb` | Deep learning experiment 4 |
| `Exp_5A.ipynb` | CNN experiments (Part A) |
| `Exp_5B.ipynb` | CNN on CIFAR-10 using PyTorch |
| `Exp_6.ipynb` | Deep learning experiment 6 |
| `Exp_7.ipynb` | RAG pipeline using LangChain + OpenAI + ChromaDB |

## 🛠️ Requirements

```bash
pip install tensorflow keras torch torchvision scikit-learn matplotlib pandas numpy
pip install langchain langchain-openai langchain-community chromadb pypdf tiktoken
```

## 🔐 API Key Setup (for Exp_7)

Exp_7 uses the OpenAI API. **Never hardcode your API key.** Set it as an environment variable:

```bash
# Linux / macOS
export OPENAI_API_KEY="your-actual-key-here"

# Windows (Command Prompt)
set OPENAI_API_KEY=your-actual-key-here
```

## 📊 Results Summary

- **Exp_1**: ANN (10 layers, 6 units each) on MNIST
  - Adam (5 epochs): ~81.7% test accuracy
  - SGD (10 epochs): ~84.1% test accuracy
- **Exp_3**: Simple CNN on MNIST → ~98.3% validation accuracy in 3 epochs
- **Exp_5B**: CNN on CIFAR-10 (PyTorch) → Loss reduced from 1.433 → 0.765 over 5 epochs

## 📝 Notes

- All notebooks were developed and tested on Google Colab
- MNIST and CIFAR-10 datasets are auto-downloaded via Keras/Torchvision
