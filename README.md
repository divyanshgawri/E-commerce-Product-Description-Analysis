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

### 3. Top 20 Brands According to Sales in a Particular Category
![Top 20 Brands by Sales](https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis/blob/main/output3.png)

This graph visualizes the top 20 brands within a specific category, showing their sales performance. It provides insights into the most successful brands in the selected category.

### 4. Most Number of Products Sold by Categories]
![Products Sold by Categories](https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis/blob/main/output4.png)

This plot represents the number of products sold across various categories. It provides a comparison of the sales volume for different categories and helps identify the most popular categories.
Here's an example of how you can describe your **NLP model** in the **README.md** to highlight its functionality and contributions to the project.

## NLP Model for Product Categorization

In this project, we developed a **Natural Language Processing (NLP) model** aimed at predicting the **category** and **sub-category** of a product description provided by a consumer. The goal was to automate product categorization and enable businesses to analyze customer feedback or product reviews more effectively. The model helps companies identify which product a user is referring to based on their description, improving customer service, inventory management, and overall business intelligence.

### **Model Overview**
The model uses **text data** (descriptions of products) as input and classifies them into predefined **categories** and **sub-categories** based on their content. This approach is particularly beneficial for businesses looking to analyze large volumes of product-related content, such as reviews or descriptions, and gain insights into which products are being talked about.

### **Steps Taken:**
1. **Data Preprocessing**: 
   - Cleaned the text data by removing unnecessary elements such as URLs, special characters, and stop words.
   - Applied **tokenization**, **lemmatization**, and **lowercasing** to standardize the text.
   - Used **TF-IDF** (Term Frequency-Inverse Document Frequency) to convert the cleaned text into numerical vectors that the model can process.

2. **Model Selection**:
   - We experimented with multiple **classification models** like **Logistic Regression**, **Random Forest**, and **Support Vector Machines (SVM)** to identify the best model.
   - Then we Selected **Logistic Regression** as our model for training.
   - The model takes the cleaned text and predicts the most probable category and sub-category using the trained classifier.

3. **Evaluation**:
   - The model's performance was evaluated using **accuracy** and **precision** metrics.
   - Cross-validation was performed to ensure the model's robustness and generalizability across unseen data.

4. **Result**: 
   - The final model is capable of classifying product descriptions with high accuracy. Businesses can now use this model to categorize products automatically based on customer-generated content such as descriptions, reviews, and feedback.

### **Features:**
- **Text Preprocessing**: Includes tokenization, removal of stop words, special characters, and URLs, and lemmatization.
- **TF-IDF Vectorization**: Converts textual data into a format suitable for machine learning models.
- **Model Flexibility**: Multiple machine learning models can be tested and evaluated for best performance.
- **Easy Integration**: The model can be integrated into existing product feedback systems or customer service platforms.

### **Future Improvements**:
- **Deep Learning**: The current model is based on classical machine learning techniques. Future work can involve training deep learning models like **LSTM** or **BERT** for better accuracy and handling more complex language patterns.
- **Domain-Specific Models**: Creating models tailored for specific industries, such as health or beauty, can improve the model’s ability to handle niche products.
- **Multilingual Support**: The model can be enhanced to work in multiple languages, making it scalable across regions and countries.

---

This section of your README will provide clear context for your NLP model, detailing its purpose, methodology, and usage for potential collaborators or employers reviewing your project.

Let me know if you'd like to adjust any details or add more explanations!
## Installation

### Prerequisites

To run this project, you need to have Python and pip installed on your system.

### Setup

1. Clone the repository:
   
   git clone https://github.com/divyanshgawri/E-commerce-Product-Description-Analysis.git
   

2. Navigate to the project folder:
   
   cd E-commerce-Product-Description-Analysis
   

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

