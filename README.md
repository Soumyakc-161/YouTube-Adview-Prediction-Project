

# 🎬 YouTube Adview Prediction Project 🚀

![alt text](<Screenshot 2024-09-19 233506.png>)

![alt text](<Screenshot 2024-09-19 233538.png>)

## 📋 Project Overview

This project focuses on predicting the number of adviews for YouTube videos based on various video metrics, such as views, likes, dislikes, comments, video duration, and published date. With the help of machine learning regression models, we aim to estimate adviews, allowing YouTube advertisers and content creators to gain insights into how much revenue they can generate from advertisements.

## 📊 Dataset Description

The dataset contains approximately **15,000 YouTube videos**, and includes the following metrics:

- 🎥 **vidid**: Unique video ID
- 👀 **views**: The number of views per video
- 👍 **likes**: Number of likes for each video
- 👎 **dislikes**: Number of dislikes for each video
- 💬 **comments**: Number of comments
- 🗓 **published**: The published date of the video
- ⏳ **duration**: The duration of the video (in minutes and seconds)
- 🏷 **category**: The category or niche of the video
- 📈 **adview**: (Target) Number of adviews

You can download the dataset [here](https://drive.google.com/file/d/1Dv-HF10AUUA03AO_cQvar462eXawk0iQ/view?usp=sharing).

---

## 🎯 Objective

To build and evaluate machine learning models to predict YouTube adview counts based on other metrics (views, likes, comments, etc.). This helps advertisers and content creators understand how different factors affect adview performance.

---

## 🛠️ Project Workflow

Here’s a breakdown of the steps and tasks followed in this project:

### 1. Data Exploration and Visualization 📊
- Explored the dataset to understand distributions and relationships between features.
- Visualized data using heatmaps and plots to check correlations.

### 2. Data Cleaning and Preprocessing 🧹
- Handled missing values and cleaned the dataset.
- Transformed categorical variables and date-related features for better modeling.

### 3. Feature Engineering 🛠️
- Extracted useful features such as year, month, day from the `published` date.
- Normalized numerical values to bring all features onto a similar scale.

### 4. Model Building 🔨
- **Linear Regression**: Simple baseline model.
- **Support Vector Regressor (SVR)**: To explore non-linear relationships.
- **Decision Tree Regressor**: Handle non-linearities and interactions.
- **Random Forest Regressor**: Ensemble method to improve accuracy.
- **Artificial Neural Network (ANN)**: Built using Keras for deep learning predictions.

### 5. Model Evaluation 📉
- Evaluated models using performance metrics:
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)
  - R² (Coefficient of Determination)
- Visualized model predictions vs actual values.

### 6. Hyperparameter Tuning 🔧
- Applied **Grid Search** to tune hyperparameters and improve model accuracy.

### 7. Saving the Model 💾
- The best-performing model was saved using `pickle` for future use.

---

## 🏆 Results and Performance

| Model                   | RMSE       | MAE        | 
|------------------------ |------------|------------|
| **Linear Regression**   |28907.83    | 3707.37    |
| **SVR**                 | 28907.8    | 3707.37    | 
| **Decision Tree**       | 35018.3    | 3059.3     | 
| **Random Forest**       |3274.69     | 25385.7    | 
| **ANN**                 | 28801.955  | 3304.26    |

The **Random Forest Regressor** outperformed the other models with the lowest RMSE and the highest R², making it the best model for predicting YouTube adviews.

---

## 🚀 How to Run the Project

### 1. Clone the Repository 📂

To get started, clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/youtube-adview-prediction.git
cd youtube-adview-prediction
```

### 2. Install Dependencies 🛠️

Make sure you have all the required libraries installed:

```bash
pip install -r requirements.txt
```

### 3. Running the Code ⚙️

You can run the Jupyter notebook or the Python scripts to reproduce the analysis and models.

For the notebook:
```bash
jupyter notebook notebooks/adview_model.ipynb
```

For the Python script:
```bash
python src/model_training.py
```

### 4. Predicting Adviews ✨

To predict adviews using the saved model, run:

```bash
python src/predict_adviews.py
```

---

## 💡 Exploratory Data Analysis (EDA)

Here’s a snapshot of the data exploration we performed:

![Heatmap](your_heatmap_image_link_here) <!-- Add your heatmap image here -->

We used a **heatmap** to visualize the correlations between features. We found that views, likes, and comments have a strong correlation with adviews.

Other visualizations such as histograms and scatter plots were also used to understand the distribution of data.

---

## 🧰 Tools and Technologies Used

- **Programming Languages**: Python 🐍
- **Libraries**: 
  - Data Handling: Pandas, NumPy
  - Visualization: Matplotlib, Seaborn 📊
  - Machine Learning: Scikit-learn, Keras 🤖
- **Version Control**: Git & GitHub
- **Model Saving**: pickle

---

---

## 📝 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

Thanks to the open-source community for providing useful tools and frameworks, and to all the contributors who maintain the datasets and libraries we rely on.

---

### 🎉 Feel free to fork, star ⭐, and contribute to this repository!

---

### Adding Images:
1. Replace the placeholder image links with actual images of your **EDA** (e.g., heatmaps, histograms).
2. Upload the images to a folder in your GitHub repository (e.g., `images/`) and link them using:

```markdown
![Image Description](images/your-image-file.png)
```










## 👤 Author

- **Soumya K C**  
  - 📧 Email: your-email@example.com  
  - 🌐 [GitHub](https://github.com/yourusername)
