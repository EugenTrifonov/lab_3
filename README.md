# Изучение влияние параметра “темп обучения” на процесс обучения нейронной сети на примере решения задачи классификации Oregon Wildlife с использованием техники
## 1.С использованием  техники обучения Transfer Learning обучить нейронную сеть EfficientNet-B0 (предварительно обученную на базе изображений imagenet) для решения задачи классификации изображений Oregon WildLife с использованием фиксированных темпов обучения 0.1, 0.01, 0.001, 0.0001
Файл train_transfer.py

![leg_2](https://user-images.githubusercontent.com/80068414/111864984-537fde80-8975-11eb-9733-20c220b1e233.png)

Метрика качества на валидации

![acc_1](https://github.com/EugenTrifonov/lab_3/blob/main/graph/epoch_categorical_accuracy.svg)

Функция потерь на валидации

![loss_1](https://github.com/EugenTrifonov/lab_3/blob/main/graph/epoch_loss.svg)

На
## 2.Реализовать и применить в обучении политики изменения темпа обучения, а также определить оптимальные параметры для каждой политики
## A)Пошаговое затухание (Step Decay)
Файл train_step_decay.py

## B)Экспоненциальное затухание (Exponential Decay)
Файл train_exp_decay.py

## 3.Анализ результатов
