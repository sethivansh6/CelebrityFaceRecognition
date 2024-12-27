![](ui_snapshot.jpg)

In this project, classified sports personalities. Restrict classification to only 5 people,
1) Maria Sharapova
2) Serena Williams
3) Virat Kohli
4) Roger Federer
5) Lionel Messi

Here is the folder structure,
* UI : This contains ui website code 
* server: Python flask server
* model: Contains python notebook for model building
* google_image_scrapping: code to scrap google for images
* images_dataset: Dataset used for our model training

Technologies used in this project,
1. Python
2. Numpy and OpenCV for data cleaning
3. Matplotlib & Seaborn for data visualization
4. Sklearn for model building
5. Jupyter notebook, visual studio code and pycharm as IDE
6. Python flask for http server
7. HTML/CSS/Javascript for UI



# Celebrity Face Recognition

This repository contains a complete pipeline for a celebrity face recognition system. It includes modules for image scraping, dataset preparation, model training, and a user interface for testing and deploying the system.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Image Scraping**: Automatically collect images from Google to create a custom dataset.
- **Dataset Preparation**: Organize images into a structured dataset.
- **Model Training**: Train a deep learning model for celebrity face recognition.
- **Interactive UI**: Test the recognition system with a user-friendly interface.
- **Server Deployment**: Host the application on a local or remote server.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/CelebrityFaceRecognition.git
   cd CelebrityFaceRecognition
```

2.Install the required Python packages:
```
bash
pip install -r requirements.txt
```

3. Set up the necessary APIs for Google image scraping.

4. Ensure you have the following prerequisites installed:

- Python 3.7 or above
- TensorFlow or PyTorch (depending on the model used)
- Flask or any other server framework for hosting



## Usage
1. Image Scraping
Run the scraper:
```
bash
python google_image_scrapping/scrape_images.py --query "Celebrity Name" --num_images 100
```
This downloads images for the specified celebrity.

2. Dataset Preparation
Organize images in the following structure:

```
images_dataset/
├── Celebrity1/
│   ├── image1.jpg
│   ├── image2.jpg
├── Celebrity2/
│   ├── image1.jpg
```

3. Model Training
Train the model:
```
bash
python model/train_model.py --dataset_path images_dataset/
```
4. Running the Server
Start the application server:
```
bash
python server/app.py
```
5. Testing
Use the UI to upload images and identify the celebrity.

## Folder Structure
```
bash
CelebrityFaceRecognition/
├── UI/                     # User interface code
├── google_image_scrapping/ # Image scraping scripts
├── images_dataset/         # Dataset of celebrity images
├── model/                  # Training and model files
├── server/                 # Backend server code
├── ui_snapshot.jpg         # UI snapshot

```

## Contributing
1. Fork the repository.
2. Create a branch for your feature:

```
git checkout -b feature-branch
Commit your changes:


git commit -m "Description of changes"
Push to your fork:


git push origin feature-branch
Open a pull request.
```
