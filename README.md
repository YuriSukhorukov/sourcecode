# sourcecode
source code

Репозиторий, заведенный в демонстрационных целях, чтобы показать исходный код части проекта. 
Репозиторий содержит исключительно код над которым я работал и не содержит никаких ресурсов. 
Суть игры заключается в разкрашивании рисунков. Рисунок представляет собой набор мешей, которые раскрашиваются 
разными материалами. Наборы материалов сожержаться в палитрах. Одна палитра - один набор материалов 
(каждыя палитра представлена отдельным набором карандашей). В целях оптимизации было реализовано запекание 
наборов карандашей в отдельный атлас, сохранение его локально.Механизм следующий: мы собираем палитру в 
инспекторе в сцене для запекания. Каждый элемент палитры может иметь отдельный цвет, текстуру (для закрашивания
рисунка узором) и шейдер. Палитры сериализуются в JSON, который сохраняется локальн. При запуске сцены 
раскраски JSON десериализуется и на его основе создается набор материалов конкретной палитры из набора палитр. 
Так же была проведена работа для адаптации интерфеса под разные разрешения, форматы и ориентации экрана.