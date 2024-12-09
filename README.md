# ADGD_URFU_4
Workshop #4

# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #4 выполнил(а):
- Иванов Денис Александрович
- РИ-230941

Отметка о выполнении заданий:
| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

## Цель работы
Научиться работать с моделью перцептрона, обучить перцептрон

## Задание 1
### Реализация перцептрона (OR, AND, NAND, XOR)
Ход работы:
- Создали новый проект и загрузили в него базовый скрипт перцептрона.
- Модифицируем скрипт так, чтобы перцептрон смог выполнять логические операции в зависимости от выбранного TrainingSet.

Операции OR, AND и NAND начиная с нескольких эпох работают корректно. Однако операция XOR - нет, так как наш перцептрон одиночный и не умеет решать нелинейные задачи.

## Задание 2
### Графики зависимости количества эпох от ошибки обучения.
Ход работы:
- Для каждой операции построим график: количество ошибок обучения - количество эпох. Поскольку количество ошибок может меняться с каждым запуском, будем брать среднее значение 5 запусков.

![image](https://github.com/user-attachments/assets/4d9cb969-ed11-44cd-853b-4be94bbcfd03)
![image](https://github.com/user-attachments/assets/9cfc139a-f859-4ac5-9249-4c2f3d9990fd)
![image](https://github.com/user-attachments/assets/a4a90a8a-bad6-482c-b451-9af1b4affa14)

Заметно, что количество ошибок резко падает, начинася с 4 эпохи, и далее стремится к нулю. Если взять во внимание, что на вход перцептрону подается датасет именно из 4 элементов, можно сделать вывод, что их количество и является минимально необходимым количеством эпох для удовлетворительной работы перцептрона.

## Задание 3
### Визуальная модель работы перцептрона.
Ход работы:
- Создаем скрипты для визуализации работы перцептрона. Суть визуализации заключается в том, что несколько кубов со случайно сгенерированными значениями (0 или 1) сталкиваются друг с другом. Их столкновение оставляет на месте куб, чьё значение равно результату работы перцептрона.

## Выводы

На основе работы с перцептроном выяснили, сколько эпох необходимо для корректной работы. Визуализировали работу перцептрона.
