# Структура проекта

## Каталог `app`

- **`logic.py`**:
  - Основная логика расчета результатов игры и определения типа победы.
  - Главная функция: `determine_winner_and_points`.

- **`main.py`**:
  - Запускает приложение на FastAPI, содержит эндпоинт для определния типа победы

- **`models.py`**:
  - Определяет Pydantic-модели для входных и выходных данных
    - **`GameResultInput`**: модель входных данных.
    - **`GameResultOutput`**: модель выходных данных.
    - Другие модели: `Board`, `BoardPoint`, и `GameWinType`.

- **`test_logic.py`**:
  - Набор тестов для проверки  `logic.py`.
  - Тестирует различные сценарии расчета очков и типа победы.

## Файлы в корневом каталоге

- **`koks.json`**:
  - Пример входных данных для победы "кокс".

- **`mars.json`**:
  - Пример входных данных для победы "марс".

- **`oin.json`**:
  - Пример входных данных для победы "оин".



