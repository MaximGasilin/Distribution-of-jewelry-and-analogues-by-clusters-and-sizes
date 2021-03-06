# Distribution-of-jewelry-and-analogues-by-clusters-and-sizes

Репозиторий содержит реализацию алгоритма распределения ювелирных изделий по торговым точкам на основании потребности. Потребность определяется не для отдельного изделия, а для кластера, который содержит как само изделие, так и заменяемые аналоги.

При поиске оптимального распределения учитываются следующие факторы:
1) На одну торговую точку должно попадать как можно меньше различных аналогов. В идеале - только один артикул товара из нескольких возможных. Но в количество самих изделий с выбранным артикулом должно быть максимально приближенным к требуемому.
2) На торговую точку желательно передавать тот аналог, который в момент распределения уже числится на остатках.
3) Для изделий имеющих размер добавляется еще один шаг алгоритма. Который пытается "оптимально" распределить имеющийся на складе объем различных размеров на ТТ так, чтобы обеспечить максимально возможное разнообразие. 

Алгоритм реализован в среде MS SQL. Использовался язык T-SQL от Microsoft.

Файл, в котором хранится сам алгоритм с демонстрацией работы на выдуманном примере -"Распределение аналогов в рамках кластера с размерами.sql"
