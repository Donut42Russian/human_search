# human_search
Поиск людей на пересеченных местностях с помощью машинного обучения. Модель написана с использованием методитики CRISP-DM.

# 2) Разведочный анализ данных (Data understanding)
  1.	Сбор данных (Data collection)
  Все данные взяты из Lacmus Drone Dataset.
  2.	Описание данных (Data description)
  Данные состоят из 406 изображений в формате .jpg и 406 YOLO описаний, хранящихся в .txt формате и содержащих координаты объекта с номером его класса. Имеется только один класс у всех объектов, обозначающий людей.
  3.	Исследование данных (Data exploration)
  Люди на изображениях носят яркую одежду, выделяющую их на фоне снега, и находятся в положении эмбриона, просто на боку или стоя. Могут находиться от одного до нескольких на одном снимке. 
  4.	Качество данных (Data quality)
  В данных отсутствуют пропуски значений, каждому изображению соответствует полная и достоверная аннотация.

# 3) Подготовка данных (Data preparation) 
  1.	Отбор данных (Data Selection)
  В рамках решения задачи по анализу изображений с одним классом нет нерелевантных атрибутов.
  2.	Очистка данных (Data Cleaning)
  В датасете отсутствуют пропущенные значения и ошибки. Все находится в единой кодировке.
  3.	Генерация данных (Constructing new data)
  Конвертация типов изображений и аннотаций, нормализация атрибутов, а также oversampling или алгоритм SMOTE не требуются.
  4.	Интеграция данных (Integrating data)
  Все данные взяты из одного источника, интеграция не нужна.
  5.	Форматирование данных (Formatting Data)
  Выбранный алгоритм работает с YOLO, форматирование не требуется.
