# NLP Kinopoisk's movies reviews 

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=blue)

Анализ ML моделей в задаче классификации отзывов 

## Модели

- **Логистическая регрессия**
- **Случайный лес**
- **XGBoost**
- **Линейный метод опорных векторов (LinearSVC)**

## Технологический стек
-   **Язык программирования**: Python 3.11
-   **Библиотеки**: NumPy, NLTK, Matplotlib, Seaborn, Scikit-learn, xgboost, pymorphy3, gensim, Pandas

## Данные
Общий размер датасета: 131669
| positive | neutral | negative |
|-----------|-----------|-----------|
| 87138  | 24704  | 19827  |

### График распределения классов 
![](images_of_results/distribution_of_reviews.png)
## Результаты

### Стемминг и TF-IDF
Обработка текста (фильтрация, токенизация, стемминг, TF-IDF)
#### **Логистическая регрессия**

![](images_of_results/LogReg_result.png)
![Матрица ошибок](images_of_results/ConfMatrix_LogReg.png)
![важные слова для каждого класса](images_of_results/MainWords_LogReg.png)

#### **Сбалансированная логистическая регрессия**

![](images_of_results/BalLogReg_ST_TF.png)
![Матрица ошибок](images_of_results/ConfMat_BalLogReg_ST_TF.png)
![важные слова для каждого класса](images_of_results/MainWords_BalLogReg_ST_TF.png)

#### **Случайный лес**

![](images_of_results/RanFor_ST_TF.png)
![Матрица ошибок](images_of_results/ConfMat_RanFor_ST_TF.png)
![важные слова](images_of_results/MainWords_RanFor_ST_TF.png)

#### **XGBoost**

![](images_of_results/XGBoost_ST_TF.png)
![Матрица ошибок](images_of_results/ConfMat_XGBoost_ST_TF.png)
![важные слова](images_of_results/MainWords_XGBoost_ST_TF.png)


### Лемматизация и TF-IDF
Обработка текста (фильтрация, токенизация, лемматизация, TF-IDF)

#### **Сбалансированная логистическая регрессия**

![](images_of_results/BalLogReg_LM_TF.png)
![Матрица ошибок](images_of_results/ConfMat_BalLogReg_LM_TF.png)
![важные слова для каждого класса](images_of_results/MainWords_BalLogReg_LM_TF.png)

#### **Линейный метод опорных векторов (LinearSVC)**

![](images_of_results/SVC_LM_TF.png)
![Матрица ошибок](images_of_results/ConfMat_SVC_LM_TF.png)
![важные слова для каждого класса](images_of_results/MainWords_SVC_LM_TF.png)

### Лемматизация и Word2Vec

#### **Сбалансированная логистическая регрессия**

![](images_of_results/BalLogReg_LM_W2V.png)
![Матрица ошибок](images_of_results/ConfMat_BalLogReg_LM_W2V.png)
![важные слова для каждого класса](images_of_results/MainWords_BalLogReg_LM_W2V.png)

