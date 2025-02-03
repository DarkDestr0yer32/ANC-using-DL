# Adaptive Noise Cancellation System Using Deep Learning  

## 📌 Project Overview  
This project focuses on enhancing audio quality by reducing background noise using deep learning. The model utilizes a **Conv1D-LSTM hybrid architecture** trained on the **Microsoft Deep Noise Suppression (DNS) dataset** to extract clean audio from noisy signals.  

## 📚 Table of Contents  
- [Introduction](#introduction)  
- [Dataset](#dataset)  
- [Methodology](#methodology)  
- [Model Architecture](#model-architecture)  
- [Results](#results)  
- [Challenges & Future Work](#challenges--future-work)  
- [Installation & Usage](#installation--usage)  
- [Contributors](#contributors)  
- [References](#references)  

## 🔍 Introduction  
Noise cancellation is essential in fields like **telecommunications, media production, and assistive technology**. Traditional methods like spectral subtraction and Wiener filtering often fail in **non-stationary noise conditions**. This project employs a deep learning-based **Conv1D-LSTM model** to reconstruct cleaner audio signals.  

## 📂 Dataset  
We utilize the **Microsoft Deep Noise Suppression (DNS) dataset**, which consists of **paired noisy and clean audio samples**. The dataset provides diverse real-world noise conditions, making it suitable for training deep learning models.  

## 🛠 Methodology  
1. **Data Preprocessing:** Convert raw audio into **Mel Frequency Cepstral Coefficients (MFCCs)** for efficient feature extraction.  
2. **Model Selection:** Employ a **Conv1D-LSTM hybrid model** for spatial and temporal feature extraction.  
3. **Training & Validation:** Monitor metrics such as **Mean Absolute Error (MAE)** and **Root Mean Squared Error (RMSE)** to evaluate model performance.  
4. **Testing & Evaluation:** Compare reconstructed clean audio with ground truth to assess noise suppression effectiveness.  

## 🏗 Model Architecture  
The model follows a hybrid **Conv1D-LSTM** structure:  
- **Conv1D Layers:** Extract spectral features.  
- **Max Pooling:** Reduce dimensionality and retain crucial information.  
- **LSTM Layers:** Capture sequential patterns in audio data.  
- **Dense Layers:** Process extracted features and reconstruct clean audio.  

## 📊 Results  
- **Low MAE and RMSE scores**, indicating strong performance.  
- **Visual waveform comparisons** demonstrate clear noise suppression.  
- Model outperforms traditional techniques in **non-stationary noise environments**.  

## 🚀 Challenges & Future Work  
### Challenges:  
- Model may **overfit on specific noise types**.  
- High-noise conditions may still degrade performance.  

### Future Enhancements:  
- Explore **transformer-based models** for better noise suppression.  
- Implement real-time processing for **streaming applications**.  

## 🔧 Installation & Usage  
### Prerequisites:  
- Python 3.x  
- TensorFlow / PyTorch  
- NumPy, Librosa, and Matplotlib  

### Installation:  
```bash  
git clone https://github.com/your-repo/Adaptive-Noise-Cancellation.git  
cd Adaptive-Noise-Cancellation  
pip install -r requirements.txt  
```  

### Running the Model:  
```bash  
python train.py  
```  

## 👥 Contributors  
- **Prathamesh Lakhotiya** (BT22ECE102)  

## 📖 References  
- Microsoft DNS Challenge Dataset (2020)  
- P. C. Loizou, "Speech Enhancement: Theory and Practice," CRC Press, 2007.  
- Zhang & Wang: Deep ANC Model for Real-Time Noise Suppression.  
- Dogra et al.: CNN-Based Noise Reduction Using MFCC Features.  
