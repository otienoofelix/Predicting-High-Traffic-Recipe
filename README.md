# Recipe Traffic Prediction

## 📌 Project Overview  
This project aims to predict which recipes are likely to generate high traffic using machine learning techniques. By analyzing features such as calories, carbohydrates, sugar, protein, and category, we evaluate the impact of these factors on recipe popularity. The study compares Logistic Regression and Random Forest models to determine the best approach for prediction.

## 📊 Data Description  
The dataset initially contained 947 rows and 8 columns, which underwent cleaning and validation to remove missing values and correct categorical inconsistencies. The final dataset consists of 895 rows.

### **Key Variables:**
- `calories`: Number of calories per recipe
- `carbohydrate`: Amount of carbohydrates (grams)
- `sugar`: Amount of sugar (grams)
- `protein`: Amount of protein (grams)
- `category`: Type of recipe
- `servings`: Number of servings
- `high_traffic`: Target variable (High or Low traffic)

## 🔍 Exploratory Data Analysis  
- High-traffic recipes were 535, while low traffic recipes were 360.
- Most recipes had low calories between 0-400, while very few recipes had calories exceeding 2000.
- During high traffic, positive relationships were observed between calories and protein, & carbohydrate and sugar, while negative relationships were observed between calories and carbohydrate, calories and sugar, carbohydrate and protein, & protein and sugar.
- Potato and vegetable were the most common recipe during high traffic, while beverages were the least common recipe during high traffic.

## ⚙️ Model Training & Evaluation  
Two models were tested:
1. **Logistic Regression**  
   - Accuracy: **77.09%**  
   - Precision: **72.86%**  
   - Recall: **69.86%**  

2. **Random Forest**  
   - Accuracy: **71.51%**  
   - Precision: **65.71%**  
   - Recall: **63.01%**  

The **Logistic Regression model** performed better in predicting high-traffic recipes.

## 📌 Key Findings  
- **Sugar** and **Servings** significantly increase the likelihood of high traffic.
- **Recipe category** has a strong impact, with certain categories receiving less engagement.
- **Calories, carbohydrates, and protein** are not significant predictors.

## 📈 Business Recommendations  
- **Optimize recipe categories** to focus on high-traffic groups.
- **Increase sugar content** (while maintaining health guidelines) to boost engagement.
- **Increase servings per recipe** to attract more views.
- **Consider additional features**, such as cooking time, ingredients, and cuisine type, for better prediction accuracy.

## 🛠️ Installation & Usage  
### **Requirements**  
- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

### **Setup**  
Clone the repository and install dependencies:  
```bash
git clone https://github.com/otienoofelix/Predicting-High-Traffic-Recipe.git
cd Predicting-High-Traffic-Recipe
```
Feel free to fork this repository, contribute, or provide feedback! 🚀

### **Author**
👤 Felix Odhiambo<br/>
📧 Contact: otienofelix@live.com<br/>
🔗 LinkedIn: https://www.linkedin.com/in/felixoodhiambo/
