# E-commerce-Product-Description-Analysis
This project is designed to predict the category and sub-category of e-commerce product descriptions provided by consumers. By analyzing the descriptions or comments, businesses can identify which product the customer is referring to, helping companies improve their product categorization, inventory management, and customer service.

## Features
**Features**
_**Category Prediction:** Predicts the primary category of the product based on the description provided by the user.
_**Sub-category Prediction:** Identifies the specific sub-category within the main category for more detailed product classification.
_**Text Preprocessing:** Handles text cleaning, including URL removal, tokenization, stopword removal, and lemmatization for improved model accuracy.
_**Scalability:** The system is designed to scale and work with large datasets for e-commerce platforms.
_**Accuracy:** The model uses advanced machine learning techniques for accurate classification of product descriptions.


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
   
   python analyze_product_descriptions.py
   

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

