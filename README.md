# 🛡️ AI Spam Detection System

A modern, intelligent email spam detection system powered by PyTorch neural networks and featuring a sleek, responsive web interface.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)
![Flask](https://img.shields.io/badge/Flask-2.0+-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## ✨ Features

- **🧠 Advanced AI Model**: Deep learning neural network built with PyTorch
- **🎨 Modern UI**: Responsive, glassmorphism-inspired web interface
- **⚡ Real-time Analysis**: Instant spam detection with confidence scoring
- **📱 Mobile Friendly**: Fully responsive design for all devices
- **🔒 Privacy Focused**: Local processing, no data stored
- **🎯 High Accuracy**: Trained on comprehensive email datasets

## 🚀 Live Demo

Experience the modern interface with features like:
- Gradient backgrounds with blur effects
- Real-time character counting
- Animated loading states
- Color-coded results with confidence bars
- Interactive safety tips and recommendations

## 🏗️ Architecture

### Model: DetectSpamV0
A feedforward neural network optimized for email classification:

```
Input Layer → Hidden Layers → Output Layer
    ↓              ↓             ↓
Text Features → Processing → Spam/Ham Classification
```

### Tech Stack
- **Backend**: Flask (Python web framework)
- **ML Framework**: PyTorch for neural network implementation
- **NLP**: NLTK for text preprocessing
- **Frontend**: Modern HTML5/CSS3 with JavaScript
- **Styling**: Custom CSS with glassmorphism effects
- **Icons**: Font Awesome 6.0

## 📁 Project Structure

```
Spam-Detection/
├── mlapp.py                 # Flask web application
├── model/
│   ├── model.py            # Neural network architecture
│   └── model_detect_spam_V0.pt  # Trained model weights
├── Preprocess/
│   └── preprocess.py       # Text preprocessing pipeline
├── templates/
│   ├── index.html          # Modern main interface
│   └── prediction.html     # Results display page
├── requirements.txt        # Python dependencies
├── Procfile               # Deployment configuration
└── README.md              # This file
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/NevroHelios/Spam-Detection.git
   cd Spam-Detection
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download NLTK data** (if needed)
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   nltk.download('wordnet')
   ```

4. **Run the application**
   ```bash
   python mlapp.py
   ```

5. **Access the web interface**
   Open your browser and navigate to `http://localhost:5000`

## 🔧 Text Preprocessing Pipeline

The system uses advanced NLP preprocessing:

1. **Tokenization**: Breaking text into individual words
2. **Cleaning**: Removing punctuation and special characters
3. **Normalization**: Converting to lowercase
4. **Stop Words Removal**: Filtering common words
5. **Stemming**: Reducing words to root forms
6. **Feature Extraction**: Converting to numerical representations

## 🎯 Model Performance

- **Architecture**: Multi-layer feedforward neural network
- **Training**: Supervised learning on labeled email datasets
- **Optimization**: Adam optimizer with learning rate scheduling
- **Evaluation**: Cross-validation with precision/recall metrics

## 🌐 Deployment

### Local Development
```bash
python mlapp.py
```

### Production Deployment
The app includes a `Procfile` for easy deployment to platforms like Heroku:

```bash
# Deploy to Heroku
heroku create your-app-name
git push heroku main
```

## 🎨 UI Features

### Modern Design Elements
- **Glassmorphism**: Frosted glass effects with backdrop blur
- **Gradient Backgrounds**: Dynamic color transitions
- **Smooth Animations**: CSS transitions and keyframe animations
- **Interactive Elements**: Hover effects and loading states

### User Experience
- **Real-time Feedback**: Character counter and form validation
- **Responsive Layout**: Adapts to all screen sizes
- **Accessibility**: WCAG compliant design
- **Performance**: Optimized loading and rendering

## 📊 API Endpoints

### GET `/`
Returns the main interface

### GET `/predict`
Analyzes email content for spam detection

**Parameters:**
- `mail` (string): Email content to analyze

**Response:**
- Renders prediction page with classification result

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**NevroHelios**
- GitHub: [@NevroHelios](https://github.com/NevroHelios)

## 🙏 Acknowledgments

- PyTorch team for the excellent deep learning framework
- NLTK contributors for natural language processing tools
- Flask community for the lightweight web framework
- Font Awesome for beautiful icons

## 📈 Future Enhancements

- [ ] Real-time model retraining
- [ ] Multi-language support
- [ ] Email attachment analysis
- [ ] Advanced threat detection
- [ ] API rate limiting
- [ ] User authentication system
- [ ] Batch processing capabilities

---

⭐ **Star this repository if you found it helpful!**