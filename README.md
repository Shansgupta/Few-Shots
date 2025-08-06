# Meta Learning-based Few-Shot Learning for Remote Sensing 🌍🚀

This project explores a hybrid meta-learning framework that integrates metric-based and memory-based strategies to tackle the challenges of low-data learning and catastrophic forgetting in remote sensing applications.

## 📚 Abstract
Traditional deep learning models struggle when labeled satellite data is scarce. To overcome this, we implement a hybrid approach combining *Relation Networks* (metric-based) with *Memory-Augmented Neural Networks (MANN)* and *Least Recently Used Access (LRUA)* (memory-based). Our framework is evaluated on three satellite datasets — *EuroSAT, **AID, and **NWPU-RESISC45* — under few-shot settings (5-way 1-shot and 5-way 5-shot). Results show promising improvements in both fast adaptation and knowledge retention, making the system ideal for real-world applications like precision agriculture, disaster response, and surveillance.

## 🛠 Tech Stack
- Python (Jupyter Notebook, Google Colab)
- PyTorch (model development and training)
- NumPy, torchvision, Matplotlib (data handling and visualization)

## 📈 Key Features
- Relation Networks for adaptive similarity learning.
- Episodic Training setup to mimic few-shot learning conditions.
- Memory-Augmented Techniques (MANN, LRUA) to combat catastrophic forgetting.
- Low-Data Simulation by using 30% of datasets during training.
- Performance Evaluation on 5-way classification tasks.

## 🗄 Datasets Used
- [EuroSAT](https://github.com/phelber/EuroSAT) — Satellite imagery over 10 land classes.
- [AID](https://captain-whu.github.io/AID/) — Aerial scenes covering 30 categories.
- [NWPU-RESISC45](https://github.com/UCAS-VG/RESISC45) — Remote sensing scenes with 45 classes.

## 🧪 Experiment Setup
- Hardware: Google Colab GPU (Tesla K80/T4).
- Training: Few-shot settings (5-way 1-shot and 5-way 5-shot).
- Preprocessing: Image resizing, normalization, random flipping, and color augmentation.
- Loss: Mean Squared Error (MSE) for Relation Networks.

## 📊 Results (Few-Shot Classification Accuracy)

| Dataset | 1-Shot | 2-Shot | 3-Shot | 4-Shot | 5-Shot |
|:--------|:------:|:------:|:------:|:------:|:------:|
| NPWU    | 37.47% | 42.27% | 33.60% | 45.87% | 39.07% |
| EURO    | 41.60% | 50.13% | 41.47% | 52.93% | 51.20% |
| AID     | 46.82% | 42.44% | 52.79% | 53.80% | 50.64% |

> Note: Results reflect preliminary runs under constrained computational settings.

## 🚀 Future Work
- Fine-tuning hyperparameters for better accuracy.
- Training over full datasets with extended episodes.
- Architectural enhancements (e.g., deeper relation modules).
- Exploration of continual learning strategies for remote sensing.

## 👨‍💻 Contributors
- *Priyanshu Gupta* (22ucs155)
- *Shantanu Gupta* (22ucc094)
- *Shashwat Agarwal* (22uec123)

Under the guidance of *Dr. Lal Upendra Pratap Singh*  
The LNM Institute of Information Technology, Jaipur
