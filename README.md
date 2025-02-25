## Comment-classifier

This Flask-based web application utilizes a fine-tuned BERT model to classify comments based on their toxicity levels. The model can identify six categories: **Toxic, Severe Toxic, Obscene, Threat, Insult,** and **Identity Hate**.
The application is packaged in a Docker container, making deployment easier and allowing users to quickly start classifying comments on any system.

## Model Performance

| Class          | Precision | Recall  | F1-Score | Support |
|---------------|-----------|---------|----------|---------|
| Toxic         | 0.98      | 0.93    | 0.96     | 3844    |
| Severe Toxic  | 0.69      | 0.70    | 0.70     | 648     |
| Obscene       | 0.92      | 0.91    | 0.92     | 2209    |
| Threat        | 0.87      | 0.78    | 0.82     | 218     |
| Insult        | 0.92      | 0.82    | 0.87     | 2253    |
| Identity Hate | 0.90      | 0.73    | 0.81     | 654     |

## Installation & Usage

Ensure **Docker** is installed on your system.

### Download Docker Image & Run the Application

```bash
docker pull FyntikUA/Comments_classifier:latest
docker run -p 5000:5000 FyntikUA/Comments_classifier
```

### Accessing the Application

Once the container is running, the app will be available at: **[http://localhost:5000/](http://localhost:5000/)**

### How to Use

1. Navigate to **[http://localhost:5000/](http://localhost:5000/)**
2. Enter a comment in the provided input form
3. Submit the comment to receive predicted toxicity labels



## Сomment-classifier

Цей веб-додаток на базі Flask використовує донавчену модель BERT для класифікації коментарів за рівнем токсичності. Модель здатна розпізнавати шість категорій: **Toxic, Severe Toxic, Obscene, Threat, Insult,** та **Identity Hate.**
Додаток упакований у Docker-контейнер, що спрощує розгортання та дає змогу швидко запустити класифікацію коментарів на будь-якій системі.

## Продуктивність Моделі
| Class          | Precision | Recall  | F1-Score | Support |
|----------------|-----------|---------|----------|---------|
| Toxic          | 0.98      | 0.93    | 0.96     | 3844    |
| Severe Toxic   | 0.69      | 0.70    | 0.70     | 648     |
| Obscene        | 0.92      | 0.91    | 0.92     | 2209    |
| Threat         | 0.87      | 0.78    | 0.82     | 218     |
| Insult         | 0.92      | 0.82    | 0.87     | 2253    |
| Identity Hate  | 0.90      | 0.73    | 0.81     | 654     |

## Встановлення та Використання

На вашому комп'ютері має бути встановлений **Docker**

### Завантаження Docker-образу та установка

```bash
docker pull FyntikUA/Comments_classifier:latest
docker run -p 5000:5000 FyntikUA/Comments_classifier:latest
```

### Доступ до Додатку

Після запуску контейнера, додаток буде доступний за адресою http://localhost:5000/

### Використання
1. Перейдіть на URL: **[http://localhost:5000/](http://localhost:5000/)**
2. Введіть коментар у відповідну форму.  
3. Надішліть коментар для отримання передбачених міток токсичності.  




