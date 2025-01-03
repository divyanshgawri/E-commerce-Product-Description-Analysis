# E-commerce-Product-Description-Analysis
This project is designed to predict the category and sub-category of e-commerce product descriptions provided by consumers. By analyzing the descriptions or comments, businesses can identify which product the customer is referring to, helping companies improve their product categorization, inventory management, and customer service.

## Features
**Features**
**Category Prediction:** Predicts the primary category of the product based on the description provided by the user.<br>
**Sub-category Prediction:** Identifies the specific sub-category within the main category for more detailed product classification.
**Text Preprocessing:** Handles text cleaning, including URL removal, tokenization, stopword removal, and lemmatization for improved model accuracy.<br>    
**Scalability:** The system is designed to scale and work with large datasets for e-commerce platforms.
**Accuracy:** The model uses advanced machine learning techniques for accurate classification of product descriptions.

## Exploratory Data Analysis (EDA)

Before building the model, we performed some **Exploratory Data Analysis (EDA)** to better understand the dataset and its structure. Below are a few visualizations that highlight important aspects of the data:

### 1. Revenue Share in Sales by Category
![Revenue Share by Category](https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis/blob/main/output1.png)

This chart shows the revenue distribution across different product categories. It helps identify the most profitable categories.

### 2. Total Sales by Top 20 Sub-categories
![Total Sales by Top 20 Sub-category](https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis/blob/main/output2.png)

This visualization shows the total sales for the top 20 sub-categories. It's useful for understanding which sub-categories contribute the most to the overall sales.

### 3. Top 20 Brands According to Sales in a Particular Category](#top-20-brands-according-to-sales
![Top 20 Brands by Sales](https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis/blob/main/output3.png)

This graph visualizes the top 20 brands within a specific category, showing their sales performance. It provides insights into the most successful brands in the selected category.

### 4. Most Number of Products Sold by Categories](#most-number-of-products-sold-by-categories
![Products Sold by Categories](https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis/blob/main/output4.png)

This plot represents the number of products sold across various categories. It provides a comparison of the sales volume for different categories and helps identify the most popular categories.

## Installation

### Prerequisites

To run this project, you need to have Python and pip installed on your system.

### Setup

1. Clone the repository:
   
   git clone https://github.com/yourusername/product-description-analysis.git
   

2. Navigate to the project folder:
   
   cd product-description-analysis
   

3. Install the required dependencies:
   
   pip install -r requirements.txt
   

4. Download necessary NLTK resources:
   python
   import nltk
   nltk.download('stopwords')
   nltk.download('punkt')
   nltk.download('wordnet')
   

## Usage

1. Place your dataset (`your_dataset.csv`) containing product descriptions in the project directory.
2. Run the following Python script to preprocess and analyze the product descriptions:
    data_analysis.ipynb
   

3. The script will clean the descriptions, perform sentiment analysis, and generate a new CSV file with the cleaned descriptions.

## Example

Here’s a sample of the cleaned description:

**Original**:  
_This Product contains Garlic Oil that is known to help proper digestion, maintain proper cholesterol levels, support cardiovascular and also build immunity. For Beauty tips, tricks & more visit https://bigbasket.blog/._

**Cleaned**:  
_product contain garlic oil help proper digestion maintain proper cholesterol level support cardiovascular build immunity beauty tip trick_

## Technologies Used
- Python
- NLTK (Natural Language Toolkit)
- Pandas
- Regular Expressions
- Scikit-leran

## Contributing
Feel free to fork this repository, create branches, and submit pull requests for improvements. Contributions are always welcome!

