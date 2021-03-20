# Изучение влияние параметра “темп обучения” на процесс обучения нейронной сети на примере решения задачи классификации Oregon Wildlife с использованием техники
## 1.С использованием  техники обучения Transfer Learning обучить нейронную сеть EfficientNet-B0 (предварительно обученную на базе изображений imagenet) для решения задачи классификации изображений Oregon WildLife с использованием фиксированных темпов обучения 0.1, 0.01, 0.001, 0.0001
Файл train_transfer.py

![leg_2](https://user-images.githubusercontent.com/80068414/111864984-537fde80-8975-11eb-9733-20c220b1e233.png)

Метрика качества на валидации

![acc_1](https://github.com/EugenTrifonov/lab_3/blob/main/graph/epoch_categorical_accuracy.svg)

Функция потерь на валидации

![loss_1](https://github.com/EugenTrifonov/lab_3/blob/main/graph/epoch_loss.svg)

По графикам метрики качества и функции потерь можно определить, что наилучшее качество достигается при темпе обучения 0.001. Выберем темп обучения равный 0.001 как оптимальный.
## 2.Реализовать и применить в обучении политики изменения темпа обучения, а также определить оптимальные параметры для каждой политики
## A)Пошаговое затухание (Step Decay)
Файл train_step_decay.py
Были реализованы 3 варианта параметров для пошагового затухания
 1)initial_lrate = 0.1
   drop = 0.4
   epochs_drop = 3.0
   
 2)initial_lrate = 0.1
   drop = 0.4
   epochs_drop = 3.0
   
 3)initial_lrate = 0.1
   drop = 0.4
   epochs_drop = 3.0
   
![leg_1](https://user-images.githubusercontent.com/80068414/111865770-02beb480-897a-11eb-8821-2c1f778f9fff.png)

Метрика качества на валидации

![acc_2](https://github.com/EugenTrifonov/lab_3/blob/main/graph/epoch_categorical_accuracy_step.svg)

Функция потерь на валидации

![loss_2](https://github.com/EugenTrifonov/lab_3/blob/main/graph/epoch_loss_step.svg)
## B)Экспоненциальное затухание (Exponential Decay)
Файл train_exp_decay.py

## 3.Анализ результатов
