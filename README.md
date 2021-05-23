# Rabin-Karp algorithm

[![CMake](https://github.com/Algorithms-and-Data-Structures-2021/semester-work-template/actions/workflows/cmake.yml/badge.svg)](https://github.com/Algorithms-and-Data-Structures-2021/semester-work-template/actions/workflows/cmake.yml)

- _Алгоритм Рабина-Карпа._
- _Это алгоритм поиска строки, который ищет шаблон, то есть подстроку, в тексте, используя хеширование._
- _Одно из простейших практических применений алгоритма Рабина — Карпа состоит в определении плагиата(ETxt, Agvego Plagiatus, Viper)._
- _Можно выполнять операцию поиска подстроки в строке._
- _Для текста длины n и шаблона длины m его среднее и лучшее время исполнения равно O(n) при правильном выборе хеш-функции, но в худшем случае он имеет эффективность O(nm)._
- _Михаэль Озер Рабин — израильский учёный в области теории вычислительных систем, математик, лауреат премии Тьюринга и многих других премий._

## Команда "чел мы..."

| Фамилия Имя    | Вклад (%) | Прозвище              |
| :---           |   ---:    |  ---:                 |
| Гордеев Илья   | 50        |  босс                 |
| Мингачев Рустам| 50        |  молокосос            |

**Девиз команды**
> _1 раз отмерь + 7 раз отмерь = 8 раз отмерь_

## Структура проекта

- [`src`](src)/[`include`](include) - реализация структуры данных (исходный код и заголовочные файлы);
- [`benchmark`](benchmark) - контрольные тесты производительности структуры данных (операции добавления, удаления,
  поиска и пр.);
- [`examples`](examples) - примеры работы со структурой данных;
- [`dataset`](dataset) - наборы данных для запуска контрольных тестов и их генерация;

## Рекомендуемые требования (Prerequisites)

1. С++ компилятор c поддержкой стандарта C++17 (например, _GNU GCC 8.1.x_ и выше).
2. Система автоматизации сборки _CMake_ (версия _3.12.x_ и выше).
3. Рекомендуемый объем оперативной памяти - не менее 8 ГБ.
4. Свободное дисковое пространство объемом ~ 2 ГБ (набор данных для контрольных тестов).

## Сборка и запуск

### Windows

#### Сборка проекта

Склонируйте проект к себе на устройство через [Git for Windows](https://gitforwindows.org/) (либо используйте
возможности IDE):

```shell
git clone https://github.com/Algorithms-and-Data-Structures-2021/semester-work-rabin-karp_chelmi.git
```

Для ручной сборки проекта в терминале введите:

```shell
# переход в папку с проектом
cd C:\Users\username\asd-projects\semester-work-rabin-karp-chelmi

# создание папки для файлов сборки (чтобы не засорять папку с проектом) 
mkdir -p build && cd build 

# сборка проекта
cmake .. -DCMAKE_BUILD_TYPE=RelWithDebInfo && cmake --config RelWithDebInfo --build . 
```

#### Генерация тестовых данных

Генерация тестового набора данных в
формате [comma-seperated values (CSV)](https://en.wikipedia.org/wiki/Comma-separated_values):
 
+ Заходим в директорию `src/dataset`
+ Находим `generate_csv_dataset.cpp`
+ Нажимаем `Run 'generate_csv_dataset'`

Тестовые данные представлены в CSV формате
[`dataset/data/dataset-example.csv`](dataset/data/dataset-example.csv))

## Источники

+ https://en.wikipedia.org/wiki/Rabin–Karp_algorithm
+ https://www.youtube.com/watch?v=oxd_Z1osgCk&t=1s
+ https://github.com/search?q=rabin_karp
