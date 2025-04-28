# PneumoScan - AI Pneumonia Detection System

PneumoScan is a web-based application that uses deep learning to detect pneumonia from chest X-ray images. This project demonstrates the application of machine learning in healthcare diagnostics.

## Features

- Upload and analysis of X-ray images for pneumonia detection
- Visualization of detection results with confidence scores
- History tracking of previously analyzed X-rays
- Detailed view of individual analysis results
- Educational information about pneumonia detection

## Tech Stack

- **Frontend**: React, TypeScript, TailwindCSS
- **Backend**: Python, Flask
- **ML/AI**: TensorFlow, Keras
- **Data Visualization**: Chart.js

## Setup Instructions

### Prerequisites

- Node.js (v14+)
- Python (v3.8+)
- npm or yarn

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/pneumoscan.git
   cd pneumoscan
   ```

2. Install frontend dependencies:
   ```
   npm install
   ```

3. Install backend dependencies:
   ```
   cd api
   pip install -r requirements.txt
   cd ..
   ```

### Running the Application

1. Start the backend API:
   ```
   npm run start-api
   ```

2. In a separate terminal, start the frontend:
   ```
   npm run dev
   ```

3. Open your browser and navigate to:
   ```
   http://localhost:5173
   ```

## Project Structure

```
pneumoscan/
├── api/                 # Backend Python API
│   ├── app.py           # Main Flask application
│   ├── model.py         # ML model definition
│   ├── utils.py         # Utility functions
│   └── requirements.txt # Python dependencies
├── public/              # Static assets
├── src/                 # Frontend React code
│   ├── components/      # Reusable UI components
│   ├── pages/           # Page components
│   ├── utils/           # Utility functions
│   ├── App.tsx          # Main application component
│   └── main.tsx         # Application entry point
├── package.json         # Node.js dependencies
└── README.md            # Project documentation
```

## Model Information

The pneumonia detection model is based on a convolutional neural network trained on the Chest X-Ray Images (Pneumonia) dataset from Kaggle. The model achieves over 90% accuracy in classifying pneumonia vs. normal chest X-rays.

**Note**: The model in this repository is for demonstration purposes. In a production environment, a more thoroughly validated model would be required.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This tool is for educational and demonstration purposes only. It should not be used for actual medical diagnosis. Always consult with a qualified healthcare professional for medical advice.