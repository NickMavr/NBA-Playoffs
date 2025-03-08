# NBA Playoff Prediction with Machine Learning

📌 Overview
This project explores the prediction of NBA playoff participation using classification models. A dataset containing NBA team statistics from the 2016-2017 season was used to train and evaluate multiple machine learning models. The goal is to provide insights into team evaluation, game strategy, and roster construction.

📊 Dataset
The dataset contains various statistical attributes of all 30 NBA teams, sourced from [Basketball Reference](https://www.basketball-reference.com/leagues/NBA_2017.html#totals-team). It includes:
- Team performance metrics (field goals, assists, rebounds, etc.)
- Advanced metrics (offensive & defensive ratings, true shooting percentage, etc.)
- Playoff participation indicator (1 if the team made the playoffs, 0 otherwise)

🛠️ Preprocessing Steps
- Removed irrelevant or redundant features (e.g., team names, rank)
- Handled multicollinearity by dropping highly correlated features
- Standardized or normalized data for models sensitive to feature scaling
- Converted relevant features to numerical formats using NumPy arrays

🤖 Machine Learning Models
Three classification models were tested:
1. **Logistic Regression**  
2. **Decision Tree Classifier**  
3. **Support Vector Classifier (Linear SVC)**  

Each model was evaluated with different normalization techniques:
- No normalization
- Standardization
- Min-max normalization

📈 Model Evaluation
To assess model performance, we used:
- **Accuracy**: Measures overall correctness of predictions
- **Precision**: Percentage of correctly predicted playoff teams
- **Recall**: Model’s ability to identify actual playoff teams
- **F1-Score**: Harmonic mean of precision and recall  

🔥 Best Results:
| Model | Normalization | Accuracy | Precision | Recall | F1-Score |
|--------|--------------|---------|---------|-------|---------|
| SVC Linear | No Normalization | **93.3%** | 91.1% | **93.3%** | **93.1%** |
| Logistic Regression | Standardization | 90% | **92.6%** | 90% | 89.6% |
| Decision Tree | Any Normalization | 90% | 91.1% | 90% | 90.1% |

🏆 Key Takeaways
- **SVC Linear (without normalization)** delivered the best accuracy and F1-score.
- **Logistic Regression (with Standardization)** was the second-best model.
- **Decision Tree** performed consistently across different normalizations.
- **Feature scaling significantly impacted model performance**, especially for logistic regression and SVC.

🔮 Future Improvements
- Try **ensemble methods** like Random Forest and Boosting techniques.
- Perform **extensive hyperparameter tuning** for further optimization.
- Integrate **additional features** (e.g., injuries, player chemistry).
- Extend analysis to **multiple NBA seasons** for better generalization.

🚀 Getting Started
### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required libraries: `pandas`, `numpy`, `scikit-learn`

💡 Contributing
Feel free to submit issues or pull requests for improvements. Contributions are welcome!

📜 License
This project is licensed under the MIT License.
