# Игровая фишка/Миниатюра (Game piece)

## О игровых фишках

![Разные миплы доступные в Tabletopia](http://help.tabletopia.com/wp-content/uploads/2015/06/meeples.png)

*Разные миплы доступные в Tabletopia*

Игровые фишки - различные объемные объекты, которые обычно делают из пластика или дерева. 

Среди кубиков, цилиндров, дисков и, конечно, миплов - самый известный символ настольных игр.

Обычно, такие объекты играют роль ресурса или персонажа, но могут быть использованы и как жетоны.

## Создание трехмерной фишки

Различные **готовые к использованию объекты доступны в Workshop**: откройте Workshop &gt; [Objects](https://tabletopia.com/workshop/objects) чтобы посмотреть все элементы, которые можжно использовать.

![create-game-piece](https://help.tabletopia.com/wp-content/uploads/2019/12/create-game-piece-13.12.19.png)

**Или создайте свои элементы** (это возможность **доступнта только пользователям Workshop Pro**, см. [Цены в Tabletopia: Планы и полкуки внутри приложения](http://help.tabletopia.com/knowledge-base/tabletopia-plans/)):

1. Нажмите **Create Object** &gt; **Game Piece** в Workshop.
2. Заполните все необходимые поля в панели справа.
3. Загрузите .OBJ файл. Ниже указаны требования к файлу.
4. Настройте текстуру, материал элемента если необходимо.
5. Нажмите **Publish**.

**Требования для 3D модели:**

* **Формат модели:** .OBJ. Одна поверхность, низкополигональная. Один .OBJ файл на модель.
* **Масштаб:** 1 единица игрового мира = 1 см (сантиметр) = 0.393 дюйма.
* **Дополнительно:** можно использовать одну карту рассеивания (diffuse texture), одну карту нормалей (normal map), одну карту свечения (glow map).
* **Рекомендуемый размер:** 512x512 пикелей.
* Центр модели должен быть расположен рядом с геометрическим центром.
* **Ограничение №1:** Количество вершины в модели должно быть в районе ~ 3-5K, максимумальное количество 30 тысяч вершин в модели (только если одна модель используется в сетапе).
* **Ограничение #2:** Физический движок Unity должен быть способен автоматически просчитывать столкновения поверхностей используя менее чем 255 полигонов (вы можете протестировать свою модель в Unity чтобы добиться этого).
* Основание модели должно быть плоским.

> **Совет:** Если вам нужен игровой элемент или игральный кубик который вы не можете сделать испольщуя другие объекты, напишите нам на [info@tabletopia.com](mailto:info@tabletopia.com).

![Трехмерные игровые элементы в игре Septikon](http://help.tabletopia.com/wp-content/uploads/2015/06/septikon_pieces.png)

*Трехмерные игровые элементы в игре Septikon*