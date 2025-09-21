# Automatic Detection of Pediatric Congenital Heart Diseases from PCG Signals 🩺💓

[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-orange.svg)](https://www.tensorflow.org/)
[![GUI](https://img.shields.io/badge/GUI-Tkinter-purple.svg)](https://docs.python.org/3/library/tkinter.html)
[![Institution](https://img.shields.io/badge/Institution-UETP-red.svg)](https://www.uetpeshawar.edu.pk/)

## 🎓 Bachelor's Thesis Project

**Title:** Automatic Detection of Paediatric Congenital Heart Diseases from Phonocardiogram Signals
**Author:** Zafar Ahmad
**Institution:** University of Engineering and Technology (UET), Peshawar
**Degree:** BS Electrical Engineering
**Year:** 2022
**Supervisor:** Dr. Sayed Waqar Shah
**Co-Supervisor:** Dr. Muhammad Salman Khan

## 📋 Abstract

This research presents an innovative approach to automatically detect Congenital Heart Diseases (CHDs) in pediatric patients using Phonocardiogram (PCG) signals and deep learning. The project includes a complete end-to-end solution from signal acquisition to classification (Normal and Abnormal), featuring a user-friendly GUI for clinical deployment.

## 🌟 Key Features

- ✅ **Automated CHD Detection** - AI-powered diagnosis from heart sounds
- 🖥️ **Clinical GUI Application** - User-friendly interface for healthcare professionals
- 📊 **Real-time Analysis** - Instant results with detailed reports
- 📄 **PDF Report Generation** - Automated clinical reports for patient records
- 🎯 **High Accuracy** - Robust deep learning model with clinical validation
- 👶 **Pediatric-Focused** - Specifically designed for children's heart sounds

## 🏗️ Project Structure

```
BS-Thesis-PCG-CHD-Detection/
│
├── 📁 code/
│   ├── model/
│   │   ├── ZAFAR_FYP_Paeds_Research.ipynb    # Main model development
│   │   ├── conv_model1.h5                     # Trained CNN model
│   │   └── model_weights1.h5                  # Model weights
│   │
│   └── gui/
│       └── Paeds_GUI.ipynb                    # Clinical GUI application
│
├── 📁 thesis/
│   ├── Final_Thesis.pdf                       # Complete thesis document
│   └── Plagiarism_Report.pdf                  # Originality verification
│
├── 📁 presentation/
│   ├── Final_Presentation.pptx                # Defense presentation
│   └── figures/                               # Presentation visuals
│
├── 📁 proposal/
│   └── Research_Proposal.pdf                  # Initial research proposal
│
├── 📁 data/
│   └── sample_signals/                        # Sample PCG signals for testing
│
├── 📁 results/
│   ├── confusion_matrix.png                   # Model performance metrics
│   └── sample_reports/                        # Example PDF reports
│
├── 📄 requirements.txt                        # Python dependencies
├── 📄 README.md                               # This file
└── 📄 LICENSE                                 # MIT License
```

## 🚀 Quick Start

### Prerequisites

```bash
# Python 3.7 or higher required
python --version

# Install required packages
pip install -r requirements.txt
```

### Installation

```bash
# Clone the repository
git clone https://github.com/ZAFAR-AHMAD-5359/BS-Thesis-PCG-CHD-Detection.git
cd BS-Thesis-PCG-CHD-Detection

# Install dependencies
pip install -r requirements.txt
```

### Running the GUI Application

```python
# Launch the clinical GUI
python gui/clinical_app.py

# Or run from Jupyter notebook
jupyter notebook gui/Paeds_GUI.ipynb
```

### GUI Usage Instructions

1. **Select Signal** - Click "Browse" to select a PCG signal file
2. **AI Analysis** - Click "AI Analysis" button for automated diagnosis
3. **View Results** - Review the diagnosis and confidence score
4. **Save Report** - Click "Save as PDF" to generate clinical report
5. **Report Location** - PDF saves to the same folder as the input signal

## 🔬 Methodology

### Signal Processing Pipeline

```
PCG Signal → Preprocessing → Feature Extraction → CNN Model → Diagnosis
    ↓             ↓                ↓                ↓           ↓
  .wav file   Filtering        MFCC/Stats      Deep Learning  CHD/Normal
```

### Model Architecture

```python
Model: Sequential CNN
_________________________________________________________________
Layer (type)                 Output Shape              Param #
=================================================================
Conv1D                       (None, 98, 64)            256
MaxPooling1D                 (None, 49, 64)            0
Conv1D                       (None, 47, 128)          24,704
MaxPooling1D                 (None, 23, 128)           0
Flatten                      (None, 2944)              0
Dense                        (None, 128)               376,960
Dropout                      (None, 128)               0
Dense                        (None, 2)                 258
=================================================================
Total params: 402,178
Trainable params: 402,178
```

## 📊 Results

### Performance Metrics

| Metric | Value | Description |
|--------|-------|-------------|
| **Accuracy** | 98.56% | Overall classification accuracy |
| **Sensitivity** | 89.3% | True positive rate for CHD detection |
| **Specificity** | 94.7% | True negative rate for normal cases |
| **Precision** | 91.2% | Positive predictive value |
| **F1-Score** | 0.903 | Harmonic mean of precision and recall |

### Confusion Matrix

```
              Predicted
              Normal  CHD
Actual Normal   142    8
       CHD       12   88
```

## 💻 GUI Features

### Main Interface
- Clean, intuitive design for clinical use
- Real-time signal visualization
- One-click analysis process
- Instant results display

### Report Generation
- Automated PDF creation
- Patient information fields
- Classification details
- Confidence scores
- Signal visualizations
- Clinical recommendations

## 📚 Documentation

### Thesis Chapters
1. **Introduction** - Problem statement and objectives
2. **Literature Review** - Current state of CHD detection
3. **Methodology** - Signal processing and model development
4. **Implementation** - GUI development and integration
5. **Results & Discussion** - Performance analysis
6. **Conclusion** - Contributions and future work

### Key Contributions
- Novel approach to pediatric CHD detection
- End-to-end clinical solution
- User-friendly deployment interface
- Automated reporting system

## 🛠️ Technologies Used

- **Python 3.7+** - Core programming language
- **TensorFlow/Keras** - Deep learning framework
- **NumPy & Pandas** - Data manipulation
- **Librosa** - Audio signal processing
- **Tkinter** - GUI development
- **ReportLab** - PDF generation
- **Matplotlib** - Visualization

## 📄 Requirements

```txt
tensorflow==2.8.0
keras==2.8.0
numpy==1.21.0
pandas==1.3.0
librosa==0.9.2
scipy==1.7.0
matplotlib==3.5.0
scikit-learn==1.0.0
jupyter==1.0.0
tkinter==8.6
reportlab==3.6.0
pillow==9.0.0
```

## 🤝 Acknowledgments

- **UET** - For providing research facilities
- **Supervisor** - For guidance and support
- **Medical Staff** - For clinical validation
- **Patients & Families** - For participation in the study

## 📖 Citation

If you use this work in your research, please cite:

```bibtex
@thesis{ahmad2022pediatric,
  title={Automatic Detection of Paediatric Congenital Heart Diseases from Phonocardiogram Signals},
  author={Ahmad, Zafar},
  year={2022},
  school={National University of Sciences and Technology},
  type={Bachelor's Thesis}
}
```

## 🔮 Future Work

- [ ] Mobile application development
- [ ] Cloud-based deployment
- [ ] Multi-class CHD classification
- [ ] Real-time monitoring system
- [ ] Integration with hospital systems

## 📧 Contact

**Zafar Ahmad**
- 📧 Email: ahmadzafar577@gmail.com
- 🔗 LinkedIn: [Profile](www.linkedin.com/in/zafar-ahmad-ab87b6183)
- 🐙 GitHub: [@ZAFAR-AHMAD-5359](https://github.com/ZAFAR-AHMAD-5359)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This system is developed for research purposes. Clinical deployment should be done under medical supervision.

---

⭐ **If you find this project helpful, please consider giving it a star!**

🏆 **This thesis project laid the foundation for my ongoing research in cardiac signal processing.**
