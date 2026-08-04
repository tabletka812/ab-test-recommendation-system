# A/B Test Analysis: Recommendation Engine

Анализ A/B-теста новой системы рекомендаций: влияние на конверсию, средний чек и удержание пользователей.

## TL;DR

- **Гипотеза:** новая модель рекомендаций повышает конверсию без потери среднего чека
- **Результат:** [впиши главный вывод одной фразой — цифра + значимость]
- **Рекомендация:** [выкатывать / не выкатывать / нужен доп. тест]

## Структура проекта

```
ab-test-recommendations/
├── README.md                    ← вы здесь
├── notebooks/
│   └── ab_test_analysis.ipynb   ← полный анализ с сохранёнными выводами
├── data/
│   ├── transactions.csv
│   └── users.csv
├── reports/
│   ├── presentation.pdf         ← презентация для нетехнической аудитории
│   └── figures/                 ← ключевые графики в png
├── requirements.txt
└── .gitignore
```

## Данные

| Файл | Описание | Строк | Период |
|---|---|---|---|
| `transactions.csv` | транзакции пользователей | ... | ... |
| `users.csv` | группа (control/test), атрибуты пользователя | ... | ... |

## Методология

1. Проверка на сплит-ошибки (SRM — sample ratio mismatch)
2. Проверка баланса групп по ключевым метрикам до теста
3. Расчёт метрик: конверсия, ARPU, средний чек
4. Статистические тесты: [z-test для пропорций / t-test / bootstrap]
5. Проверка на гетерогенность эффекта по сегментам

## Ключевые результаты

| Метрика | Control | Test | Δ | p-value |
|---|---|---|---|---|
| Конверсия | ... | ... | ... | ... |
| Средний чек | ... | ... | ... | ... |
| ARPU | ... | ... | ... | ... |

Графики — в `reports/figures/`, полный разбор — в `notebooks/ab_test_analysis.ipynb`.

## Как воспроизвести

```bash
git clone https://github.com/<your-username>/ab-test-recommendations.git
cd ab-test-recommendations
pip install -r requirements.txt
jupyter notebook notebooks/ab_test_analysis.ipynb
```

## Стек

Python, pandas, scipy/statsmodels, matplotlib/seaborn, Jupyter

## Автор

[Имя] · [ссылка на LinkedIn/сайт] · [email]
