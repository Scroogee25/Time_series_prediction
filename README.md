# Time Series Prediction — Daily Revenue Forecast

Задача: прогноз `total_amount_net` по дням (2022-01-01…2023-12-31, 730 наблюдений).  
Показываю два бейзлайна: **Prophet** (интерпретируемый, календарные фичи) и **LightGBM** (сильный табличный, лаги/роллинги).

## Данные
`datasets/daily.csv` со столбцами:
- `service_date` (YYYY-MM-DD)
- целевая: `total_amount_net`
- дополнительные фичи: `unique_patients`, `hospital_amount`, `non_hospital_amount`, `unique_service_codes`, `total_records`, лаги/EMA/роллинги
