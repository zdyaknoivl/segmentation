# Проект по сегментации новообразований на медицинских снимках

Этот проект посвящен разработке системы сегментации новообразований на медицинских снимках с использованием сегментационных нейросетей. Сегментация новообразований является важной задачей в медицинском образовании и диагностике, которая помогает визуализировать и выделить области интереса для анализа и лечения.

## Архитектуры нейросетей

В проекте использовались следующие архитектуры сегментационных нейросетей:

1. SegNet: SegNet - это глубокая сверточная нейронная сеть, разработанная специально для задач сегментации. Она основана на энкодер-декодер архитектуре и содержит пулинговые слои, которые помогают снизить размерность и сохранить пространственную информацию.
2. UNet: UNet - это еще одна популярная сверточная нейронная сеть для сегментации. Ее архитектура также основана на энкодер-декодер подходе, но с добавлением skip-соединений, которые помогают передавать информацию между энкодером и декодером.
3. UNet2: UNet2 - это модификация UNet с улучшенной архитектурой.

## Описание процесса

1. Подготовка данных: Для обучения и оценки производительности моделей были использованы различные медицинские снимки, включающие новообразования. Данные были предварительно обработаны.
2. Разработка моделей: Были реализованы SegNet, UNet и UNet2 с использованием PyTorch. Каждая модель была обучена на размеченных данных для сегментации новообразований.
3. Обучение и настройка моделей: Обучение моделей производилось с использованием оптимизации градиентным спуском и различными функциями потерь, такими как binary cross-entropy loss, dice loss и tversky loss.
4. Оценка производительности: После обучения моделей была проведена оценка их производительности на отложенных тестовых данных.
