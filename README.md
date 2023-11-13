# DocuGuard: Whitener and Overwriting Detection

DocuGuard is a web application designed to detect the use of whitener and instances of overwriting on scanned document images. Using a custom-trained machine learning model, DocuGuard can identify tampered areas and highlight them with bounding boxes. This project is ideal for document verification processes, ensuring the authenticity and integrity of paperwork.
## Application Interface

Below is the web interface of DocuGuard where users can upload documents to be analyzed:

![DocuGuard Interface](images/whitener_interface.png)
![DocuGuard Interface](images/whitener_sample.jpeg)
![DocuGuard Interface](images/overwriting_interface.png)
![DocuGuard Interface](images/overwriting_sample.png)

## Features

- **Custom Machine Learning Model**: Built with a dataset specifically created to recognize whitener and overwriting on documents.
- **Interactive Web Interface**: A simple and intuitive web interface for users to upload and check documents.
- **Real-time Detection**: Quickly processes documents and visualizes the results on the web page.
- **Open Source**: Fully open-source with the flexibility to extend or modify to suit different requirements.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.6 or higher
- Flask
- Ultralytics YOLO (for the machine learning model)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/ajbatth/docuguard.git
cd docuguard
```

2. Install the required Python packages:
```bash
pip install -r requirements.txt
```

### Usage

1. Start the Flask web server:
```bash
python3 predict_api.py --device cpu
```

2. Open your web browser and go to `http://127.0.0.1:3000/`.

3. Upload a document image using the web interface.

4. View the results as the application detects and highlights any areas with whitener or overwriting.

## How It Works

- **Data Preparation**: The machine learning model was trained on a custom dataset created specifically for detecting tampering in documents.
- **Training**: The model was trained on Google Colab using the YOLO (You Only Look Once) architecture provided by Ultralytics.
- **Integration**: The trained weights were integrated into a Flask web application, allowing for seamless inference and user interaction.



