# 🗜️ IMG lite Image Compressor & Resizer
[IMG Lite](https://img-lite.streamlit.app/)
A fast, lightweight web application built with Python and Streamlit that allows users to batch compress images to an exact target file size (KB) or resize their pixel dimensions. 

This tool is entirely private and processes everything in your machine's RAM without saving files to the hard drive.

## ✨ Features

- **Batch Processing:** Upload and process multiple images at the same time.
- **Target Size Compression:** Specify an exact target size (e.g., 50 KB), and the app will intelligently lower the quality and scale down the image until it fits the requirement.
- **Smart Resizing:** Set maximum pixel dimensions. The app uses `Lanczos` resampling and maintains the original aspect ratio so your images never stretch or distort.
- **Bulk Download:** Downloads single files normally, or automatically packages multiple processed images into a `.zip` file for 1-click downloading.
- **Format Support:** Works with `JPG`, `JPEG`, `PNG`, and `WEBP`. (Automatically handles PNG-to-JPEG transparency flattening).

## 🛠️ Tech Stack

- **Python 3.8+**
- **Streamlit:** For the web interface.
- **Pillow (PIL):** For image processing and resampling.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### 1. Clone or Download the Repository
Ensure you have the project files (`app.py` and `.gitignore`) in a dedicated folder.

### 2. Create a Virtual Environment
It's highly recommended to use a virtual environment to manage dependencies.

**Windows:**
```
python -m venv venv
venv\Scripts\activate
```
**Mac/Linux:**
```
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
With your virtual environment activated, install the required Python packages:
```
pip install streamlit pillow
```
### 4. Run the Application
Start the Streamlit development server:
```
streamlit run app.py
```
The application will automatically open in your default web browser at http://localhost:8501
🖥️ Usage
Open the app in your browser.

Choose your operations:

Compress File Size: Check this and enter your desired maximum file size in KB.

Resize Pixel Dimensions: Check this and enter your maximum Width and Height in pixels.

Drag and drop one or multiple images into the uploader.

Click "🚀 Process Images".

Preview the results and click the download button to save your files!

📄 License
This project is open-source and available under the MIT License.
