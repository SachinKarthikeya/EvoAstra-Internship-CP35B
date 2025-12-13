# Skill Evaluation Assessment - Major Project - Minor Project

## Skill Evaluation Assessment

The skill evaluation assessment was based on an E-commerce Customer Behavior dataset, which tested:
- Data Understanding and basic Analysis
- Customer Analysis and Business Intelligence
- Research Methodology and Predictive Analysis
- Professional Communication and Leadership Skills

## Major Project - Image Captioning using Hybrid CNN-LSTM Model

The major project aims to generate descriptive captions for the given images by implementing a hybrid Convolutional Neural Network (CNN) - Long-Short Term Memory (LSTM) models. The project involves essential steps like Image pre-processing, Captions cleaning and Tokenization, Image Features Extraction, Model Building, Training and Evaluation.

## Workflow

- Loaded the Flickr8k dataset, which contains 8091 images of different scenarios with 5 captions for each scenario
- Pre-processed the images like resizing, reshaping, etc.
- Extracted the features of pre-processed images using the VGG16 model and stored them for quicker and future use
- Loaded the captions text file and pre-proccesed the captions like deleting digits, special characters, additional spaces, tokenizing and added start and end tokens to the beginning and end of each caption
- Split the dataset into 80% for training and 20% for testing purposes
- Defined a batch generator which includes a padding sequence to normalizes the size of all captions to the max size for better results.
- Built the model using Tensorflow encoder-decoder architecture
- Trained the model over 20 epochs
- Saved the trained model
- Evaluated the model using Bilingual Evaluation Understudy (BLEU) scores.

## Minor Project - Web Scraping for Data Extraction and Presentation

THe mini project aims to extract and analyze car details from AckoDrive website using Web Scraping technique. This project covers essential steps like Website Research and Planning, Data Extraction, Cleaning and Presentation.

## Workflow

- Researched the website and focused on gathering the data of Maruti Suzuki cars from Mumbai, covering key details such as **Name**, **Fuel Type**, **Transmission**, **Price**, **Year**, **Rating** and **Location**
- Planned to extract the specific data using the combination of **Selenium** and **BeautifulSoup** because:
  - AckoDrive uses Javascript to load pages dynamically, Selenium is preferred to extract real-time data
  - BeautifulSoup is fast at parsing HTML, supports CSS selectors and extracts clean text data.
- Visited the website and loaded the car cards, which contain the content of each card
- Took a HTML tag of one car card, so that it can find others with the same CSS class and extracted the data of necessary details in text format
- Created a dictionary in Python for each car's content, which is later updated to an empty list
- Converted the list into a DataFrame and saved it in the form of a CSV file
- Cleaned the dataset like removing empty columns and replacing empty columns with "NaN"
