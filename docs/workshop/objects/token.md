# Жетон\Токен (Token)

## О жетонах (токенах)

Жетоны обладают толщиной, поэтому они обычно используются как ресурсы или персонажи. Уникальное свойство жетона - способность использовать вертикальные и горизонтальные изображения одновременно. В этом случае игроки видят плоское изображение, когда смотрят сверху, но при изменении угла камеры, жетон становится вертикально стоящей фигурко на подставке.

**Возможности:**

* **Размер:** до 1600&#215;1600 мм
* **Толщина:** от 0.2 до 50 мм
* **Поддержка сложной формы:** да
* **Возможность создать стопку:** да
* **Боковой цвет:** да

![Жетоны игроков в игре Five Seals of Magic в вертикальной и горизонтальной формах](http://help.tabletopia.com/wp-content/uploads/2015/06/5_seals_tokens.png)

*Жетоны игроков в игре Five Seals of Magic в вертикальной и горизонтальной формах*

## Использование жетонов

Варианты использования жетонов:

 ![Уникальные жетоны монет и товаров в игре Cuba](http://help.tabletopia.com/wp-content/uploads/2015/06/cuba_custom_tokens.png)

 *Уникальные жетоны монет и товаров в игре Cuba*

* **Жетоны или фигурки персонажей.** Одно из основных применений этого объекта - использовать как фигурку персонажа в игре. Вы можете задать толщину и боковой цвет при необходимости.
    
    Если вы укажете вертикальное изображение для жетона, оно будет использоваться, если вы смотрите на жетон со стороны.
    
    Имейте ввиду, что переднее вертикальное изображение показывается с любого угла обзора, если жетон лежит передней стороной вверх. Изображение изменится когда вы перевернете его на другую сторону.

* **Плоский горизонтальный жетон.** Используйте этот объект как плоский и толстый жетон ресурсов любой формы (используя альфа-канал), например, вместо использования простых кубиков.

* **Плоский вертикальный жетон.** Миплы или любой другой стоящий компонент может быть представлен как жетон. Вертикальный жетон во многом похож на горизонтальный, но вместо размещения на одной из плоских сторон, они стоят вертикально.

> **Совет:** Каждый объект в Tabletopia обладает звуком, который воспроизводится когда что-либо происходит с объектом. Например, когда положить или взять жетон в игре *Five Seals of Magic* звучит звук ‘испарения’, персонажи разговаривают, когда игрок берет их, и т.д. Вы можете заменить стандартные звуки любыми уникальными. Представьте, что играя боевым роботом вы слышите звук металлических шарниров, или играя карту "Атака ракетой "земля-воздух" вы слышите звук запуска ракеты. Подробнее смотите в статье [Нестандартные звуки](../enhance/custom-sounds.md).

* **Самодельные кубики или диски.** Если вам нужен диски или кубики разных размеров или форм, но их нет в Workshop, вы можете сделать свои и подогнать их под свои нужды используя объект Token.
    
    ![Жетоны игроков для иллюстрации состояния и отмечания зоны игрока в игре Comparity](http://help.tabletopia.com/wp-content/uploads/2015/06/comparity_tokens.png)

    *Жетоны игроков для иллюстрации состояния и отмечания зоны игрока в игре Comparity*

* **Жетоны сложных форм.** Чтобы сделать жетоны сложных форм, также используйте объект Token

* **Фигурка игрока.** Иногда необходимо отметить временную или подвижную зону игрока. Вы можете создать жетон для этой задачи. Жетоны с разным изображением на своих сторонах добавляют возможность указывать текущее состояние игрока, например одна сторона иллюстрирует активное состояние во время хода игрока, и другая сторона - неактивная, во время хода другого игрока.

![Токены с разными сложными формами в игре Terra Mystica](http://help.tabletopia.com/wp-content/uploads/2015/06/terra_mystica_tokens.png)

*Токены с разными сложными формами в игре Terra Mystica*

## Создание токенов со сложной формой

Здесь вы узнаете как создать токены со сложной формой, например токен в стиле игры Pac-man.

![25](http://help.tabletopia.com/wp-content/uploads/2015/06/25.png)

Предположим у вас уже есть изображение для токена на белом фоне. Откройте ее в любом графическом редакторе который может создавать файлы .PNG.

![31](http://help.tabletopia.com/wp-content/uploads/2015/06/31.png)

1. Измените размер изображения принимая во внимание то, что стандартные пропорции это 10 пикселей на 1 миллиметр. Мы изменяем размер изначального изображения до квадрата со стороной 400 пикселей (40 мм x 10 пикс/мм).

2. Удалите фон и добавьте прозрачности. Имейте ввиду, что Tabletopia не поддерживает полупрозрачность.

3. Сохраните изображение в .PNG файл.

4. Если необходимо, создайте изображение для задней стороны токена и сохраните в другой файл.

5. Добавьте изображение токена в Tabletopia (подробнее читайте в статье [Регистрация игрового объекта](how-to-fill-in-an-object-form.md)) и используйте в своей игре.

Имейте ввиду, что область с острыми углами поддерживает только визуальную прозрачность. Так в изображении из этого примера область рта будет взаимодействовать с другими объектами как часть жетона, несмотря на то, что она прозрачна. Это ограничение Tabletopia. Помните об этом, когда создаете свои объекты.
Тем не менее прозрачные области вокруг круглой стороны токена обрабатываются Tabletopia как несуществующие.

![32](http://help.tabletopia.com/wp-content/uploads/2015/06/32.png)