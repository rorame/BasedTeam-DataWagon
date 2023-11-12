## Описание файлов

`data_preprocessing.ipynb` - предобработка данных, генерация новых предикторов
`catboost_model.ipynb` - финальная модель предсказания
`catboost_feature_importance.ipynb` - влкад предикторов финальной модели в предсказание
`improved_baseline_model.ipynb` - улучшенная базовая модель


## Бизнес ценность

* В основе нашей модели лежит алгоритм градиентного бустинка
* Итоговый скор модели на 8 утра 12 ноября - __0.53645__
* За основу были взяты наиболее понятные (числовые) признака, которые наиболее полно и просто объясняют процесс отправки вагона на плановый ремонт 
* Главные Фичи: остаточный пробег, кол-во дней до и после планового ремонта, кол-во дней после ремонта в депо, количество дней после капитального ремонта,  вид ремонта
* Второстепенные Фичи: предельная грузоподъемность, кол-во дней после постройки, кол-во дней до ликвидации, средний пробег за день и месяц, объем кузова, норма пробега
