# Определение уязвимых групп населения
## Итоговый проект  обучения Skillfactory Data Science 

### Оглавление
[1.Задачи]
[2.Этапы работы над проектом]
[3.Результаты и выводы]

### 1. Задача

- кластеризовать регионы России и определить, какие из них наиболее остро нуждаются в помощи малообеспеченным/неблагополучным слоям населения;
- описать группы населения, сталкивающиеся с бедностью;
- определить:
   - влияет ли число детей, пенсионеров и других социально уязвимых групп на уровень бедности в регионе;
   - связаны ли уровень бедности/социального неблагополучия с производством и потреблением в регионе;


### 2. Этапы работы над проектом

- компиляция данных.
- построение ML-модели кластеризации.
- описание кластеров, анализ зависимостей.

### 3. Результаты и выводы

* Проведено считывание экономических и демографических данных из предоставленных файлов различного формата и из дополнительных источников. На основе полученных датасетов сформирована финальная таблица по срезу 2020 г. 

* В качестве критериев для группировки регионов в кластеры с близкими параметрами выбраны признаки, отражающие социально-экономическое благополучие субъектов федерации. Для проведения кластеризации выбраны независимые характеристики: 
  - номинальную заработную плату, нормированную на прожиточный минимум в регионе;
  - валовый региональный продукт в логарифмической шкале;
  - объем розничной торговли на человека, нормированный  на прожиточный минимум в регионе;
  - жилую площадь на человека;
 
* С помощью различных внутренних метрик кластеризации оценено оптимальное количество кластеров (три). Построена базовая модель (k-means). Выполнено PCA-понижение размерности (3 главных компоненты, объясняющие 90% дисперсии). Протестированы различные алгоритмы кластеризации, из них на основе метрик и визуализации признакового пространства выбран оптимальный ("k-means на PCA-компонентах"), регионам присвоены соответствующие метки. Продемонстрирована устойчивость общей структуры кластеров при использовании различных алгоритмов кластеризации. 

* Дано описание характерных особенностей полученных кластеров:
  - среднестатистические регионы;
  - регионы "комфорт"
  - бизнес-регионы.

* Проведен анализ социально-демографических групп населения, показывающий, что наиболее уязвимой группой населения по финасовым показателям являются семьи с детьми. 
