# Александр Ковтуненко

Кросс-компетентный специалист: инженер-теплотехник с 18-летним опытом в энергетике и Data Scientist.

В 2022–2023 годах прошёл программу профессиональной переподготовки **«Специалист по Data Science плюс»** (Яндекс Практикум, 630 часов) и защитил 19 учебных проектов — от исследовательского анализа данных и классического машинного обучения до компьютерного зрения, обработки естественного языка, временных рядов, SQL и PySpark.

## Навыки

- **Языки и анализ данных:** Python (pandas, NumPy, SciPy), SQL (PostgreSQL), PySpark
- **Машинное обучение:** scikit-learn, CatBoost, LightGBM, XGBoost, Optuna, SHAP, PHIK
- **Нейронные сети:** PyTorch, TensorFlow/Keras, transformers, компьютерное зрение, NLP
- **Инструменты:** Git, Jupyter, Matplotlib, Seaborn, SQLAlchemy, ONNX Runtime, Linux

## Личные проекты

**[news-classifier-rubert](https://github.com/WiMean/news-classifier-rubert)** — NewsMiner, агрегатор новостных заголовков с локальной ML-моделью. Кейс проекта (описание, архитектура, результаты; код и веса модели не публикуются): fine-tuning `DeepPavlov/rubert-base-cased` (11 классов, заголовок + описание, 96 токенов), обучение на трёх сидах с выбором по macro-F1, псевдоразметка неразмеченного пула (+2 194 примера), веса классов и label smoothing, экспорт в ONNX INT8 с офлайн-инференсом на устройстве. На отложенной выборке (903 примера): **accuracy 85,2 %, macro-F1 0,778**, согласие INT8 с FP32 — **99 %**.

Полный цикл ML-фичи: разметка и балансировка данных, обучение и подбор сидов, INT8-квантование, контрактные тесты модели, fallback на rule-based классификатор.

**[brigade-planner](https://github.com/WiMean/brigade-planner)** — «Планировщик работ бригады»: офлайн-приложение для мастера участка на Expo SDK 54, React Native 0.81 и TypeScript. Годовой график ТО и ППР, недельные поездки бригады, пропуска, фотофиксация, отчёты в XLSX и PDF. В релизной сборке заблокировано разрешение `INTERNET` — приложение физически не имеет доступа к сети. 30 экранов, ~19 600 строк кода, 10 миграций схемы, 13 скриптов автоматической проверки, весь SQL прогоняется в Node без эмулятора. Кейс проекта (код не публикуется).

## Учебные проекты Яндекс Практикума

| Проект | О чём | Репозиторий |
|---|---|---|
| **Исследование рынка российского кинопроката** | EDA рынка российского кинопроката: сборы, господдержка, интерес зрителя | [studies-cinema-market-eda](https://github.com/WiMean/studies-cinema-market-eda) |
| **Исследование объявлений о продаже квартир** | EDA объявлений о продаже квартир: аномалии, цена за м², влияние факторов | [studies-apartments-eda](https://github.com/WiMean/studies-apartments-eda) |
| **Прогнозирование оттока клиентов «Бета-Банка»** | Классификация оттока клиентов банка: F1 0,63, AUC-ROC ≈ 0,86 | [studies-bank-churn](https://github.com/WiMean/studies-bank-churn) |
| **Рекомендация тарифов мобильного оператора** | Подбор тарифа мобильного оператора по поведению клиента: accuracy 0,82 | [studies-tariff-recommendation](https://github.com/WiMean/studies-tariff-recommendation) |
| **Прогнозирование отказа от брони в сети отелей «Как в гостях»** | Прогнозирование отказа от брони в отеле: CatBoost, Optuna, SHAP | [studies-hotel-booking-cancellation](https://github.com/WiMean/studies-hotel-booking-cancellation) |
| **Выбор локации для бурения скважины** | Выбор региона для бурения скважин: регрессия и bootstrap-анализ рисков | [studies-oil-well-location](https://github.com/WiMean/studies-oil-well-location) |
| **Определение стоимости автомобилей** | Определение стоимости автомобиля: CatBoost RMSE 1583 против 2362 у линейной модели | [studies-car-price-regression](https://github.com/WiMean/studies-car-price-regression) |
| **Прогнозирование заказов такси (временные ряды)** | Прогнозирование заказов такси: временные ряды, RMSE 32,4 | [studies-taxi-orders-time-series](https://github.com/WiMean/studies-taxi-orders-time-series) |
| **Защита персональных данных клиентов** | Защита персональных данных клиентов обратимым преобразованием признаков | [studies-personal-data-protection](https://github.com/WiMean/studies-personal-data-protection) |
| **Классификация токсичных комментариев для «Викишоп» (NLP)** | Классификация токсичных комментариев: TF-IDF, LightGBM, BERT, F1 0,77 | [studies-wikishop-toxic-comments](https://github.com/WiMean/studies-wikishop-toxic-comments) |
| **Определение возраста покупателей по фотографии (CV)** | Определение возраста покупателей по фотографии: ResNet50, MAE 6,4 года | [studies-customer-age-cv](https://github.com/WiMean/studies-customer-age-cv) |
| **Оценка риска ДТП по выбранному маршруту** | Оценка риска ДТП по маршруту: LightGBM, XGBoost, Optuna, SHAP | [studies-car-accident-risk](https://github.com/WiMean/studies-car-accident-risk) |
| **Продвинутый SQL** | Продвинутый SQL: JOIN, CTE, оконные функции (PostgreSQL) | [studies-advanced-sql](https://github.com/WiMean/studies-advanced-sql) |
| **Предсказание стоимости жилья в Калифорнии (PySpark)** | Стоимость жилья в Калифорнии на PySpark: R² 0,648 | [studies-california-housing-spark](https://github.com/WiMean/studies-california-housing-spark) |
| **Прогнозирование температуры плавления стали (промышленность)** | Прогноз температуры стали: MAE 6,11 °C, CatBoost / LightGBM / XGBoost | [studies-steel-temperature](https://github.com/WiMean/studies-steel-temperature) |
| **Поиск изображений по текстовому запросу (PoC)** | PoC поиска изображений по текстовому запросу: CLIP, ResNet, BERT | [studies-image-search-clip](https://github.com/WiMean/studies-image-search-clip) |
| **Прогнозирование оттока клиентов оператора связи (финальный проект)** | Финальный проект: отток клиентов оператора связи, ROC-AUC 0,86 | [studies-telecom-churn-final](https://github.com/WiMean/studies-telecom-churn-final) |
| **Прогнозирование температуры поверхности звёзд** | Температура поверхности звёзд: нейронная сеть, RMSE ≈ 5108 K | [studies-star-temperature](https://github.com/WiMean/studies-star-temperature) |
| **Определение уровня английского языка по тексту (мастерская NLP)** | Определение уровня английского языка (A2–C1) по тексту | [studies-nlp-english-level](https://github.com/WiMean/studies-nlp-english-level) |

## Контакты

- Email: remarkmarcus@gmail.com
- GitHub: [@WiMean](https://github.com/WiMean)

---

*Открыт к предложениям в области анализа данных и машинного обучения, а также к инженерным позициям в энергетике.*
