# Power BI анализ и визуализации данных


![power-bi-banner](https://user-images.githubusercontent.com/43387913/56744961-1e1ae800-6782-11e9-9b1a-175dd66fba7d.jpg)


#### Описание данных:

Исходные данные содержаться в двух файлах

1. Файл "Клиенты". Содержит данные об участниках программы. В таблице ниже указаны столбцы исходной таблицы и описание содержимого каждого столбца.

| Данные          | Описание                                                                              |
|-----------------|---------------------------------------------------------------------------------------|
| ID              | Порядковый номер участника программы                                                  |
| Номер участника | Уникальный номер участника                                                            |
| Имя             | Вносится участником самостоятельно                                                    |
| Дата создания   | Дата и время регистрации участника в программе лояльности                             |
| Дата рождения   | Дата рождения участника                                                               |
| Пол             | Пол участника                                                                         |
| Город           | Город проживания участника. Вносится участником самостоятельно. Присутствуют опечатки |

2. Файлы "Продажи". Содержит данные о продажах. В таблице ниже указаны столбцы исходной таблицы и описание содержимого каждого столбца.

| Данные             | Описание                                                                                       |
|--------------------|------------------------------------------------------------------------------------------------|
| Город              | Город местонахождения ресторана. Отличается от города регистрации участника из файла "Клиенты" |
| Название ресторана | Название ресторана                                                                             |
| Номер ресторана    | Уникальный номер ресторана                                                                     |
| ID транзакции      | Уникальный номер транзакции                                                                    |
| Номер участника    | Уникальный номер участника                                                                     |
| Тип блюда          | Категория блюда                                                                                |
| Код блюда          | Уникальный код блюда                                                                           |
| Название блюда     | Название блюда                                                                                 |
| Цена блюда         | Цена продажи блюда с НДС                                                                       |
| Количество         | Количество                                                                                     |
| Дата транзакции    | Дата транзакции                                                                                |
| Сумма чека         | Сумма чека                                                                                     |


#### Описание отчетов:

  НДС равен 18%

1. Общий отчет по участникам программы. 
 * Показатели:
   * Кол-во уникальных покупателей;
   * Кол-во покупок (транзакций);
   * Средний чек, без НДС;
   * Частоту покупок.
 * Фильтры:
   * По городам проживания участников программы;
   * По периодам (месяц-год) вступления участника в программу.
  
2. Отчет по продажам в разрезе точек продаж.
* Показатели:
   * Среднемесячное кол-во покупок (транзакций);
   * Средний чек, без НДС;
   * Доля активных участников от общего кол-ва участников;
   * Продажи (выручка), без НДС.
* Фильтры:
   * По городам нахождения ресторанов;
   * По названиям ресторанов;
   * По месяцам продаж.

3. Отчет по активности для разных типов клиентов.
* Показатели:
   * Среднемесячное кол-во покупок (транзакций);
   * Доля активных участников от общего кол-ва участников;
   * Рейтинг блюда;
   * Средняя цена блюда.
* Фильтры:
   * По городам нахождения ресторанов;
   * По годам;
   * Типам клиентов. 
     * Возможны три типа клиентов:
     * i. Light (меньше 0,5 визитов в месяц за все время, когда собирались данные)
     * ii. Medium (от 0,5 и менее 1,5 визитов в месяц за все время, когда собирались данные)
     * iii. Hard (от 1,5 визитов в месяц за все время, когда собирались данные)
   * По возрасту клиентов. Возможны следующие группы:
     * i. До16
     * ii. От16до24
     * iii. От24до35
     * iv. От35до50
     * v. От50


## Все данные отчетов тестовые
