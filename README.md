Project Evoluo
==============

С помощью класса Screen осуществляется вывод на экран
Класс Curses -- выводит в консольку. Рекомендуется ставить шрифт 8х8
Класс Layer -- суперкласс слоя (любого). Обязательными являются модули step (вызывается при каждом шаге, изменяет параметры окружения)
Класс LayerObjects -- в отличии от Layer, содержит в себе объекты, икоторые взаимодействуют между собой и другими объектами.
Класс LayerViscosity -- Замедляет объекты
Класс Mind -- мозги бота. Принимают на вход инфу об окружающем мире, выдают то, что должен бот делать.
Класс Object -- Объект.
Хар-ки:
  pos -- положение в прострастве
  _energy -- энергия на данный момент
  _max_energy -- максимальная энергия
  speed -- текущая скорость
  _accel -- текущее ускорение
  radius -- радиус объекта
  mass -- масса = радиус^2
  status --  статус объекта, выставляется в _change_state()
  _strong -- Характеристика защиты и силы
  _mind -- переменная-класс мозгов
  _attack -- сила атаки
  _attack_range -- дальность атаки
Класс ObjectBot -- "Живой" объект.