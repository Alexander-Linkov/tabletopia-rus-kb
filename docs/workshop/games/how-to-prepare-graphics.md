# Подготовка изображений

Изображения играют важную роль в большинстве настольных игр, предоставляя необходимую информацию, помогая в использовании компонентов, поддерживая тему игры и создавая атмосферу.

![1](http://help.tabletopia.com/wp-content/uploads/2015/06/1.png)

Цель Tabletopia - позволить авторам и издателям быстро адаптировать игровую графику из стандартной предпечатной графики и ПнП файлов. Обычно можно создать игру всего за несколько часов. Подробнее читайте в статье [Как создать игру](how-to-create-game.md).

Однако вы можете пойти дальше и создать объекты, которых нет в физической версии игры, например заменить абстрактные деревянные кубы-ресурсы на приятные жетоны или даже 3d элементы, разрабортать особые зоны игроков и проч. Больше читайте в статье [Советы по улучшению визуального стиля игры](http://help.tabletopia.com/knowledge-base/visual-design-guide/).

В этой статье вы найдете особенностм подготовки изображений в Tabletopia и некоторые полезные советы.

## Файлы изображений

Варианты изображений, которые могут быть у каждого игрового дизайнера следующие:

* **Предпечатные файлы.** Игра уже издана и у вас есть изображения, использованные для печати.

* **ПнП.** Игра не издана, но у вас есть изображения, использованная для подготовки физических прототипов.

* **Нет изображений.** В этом случае вам придется всё создавать с нуля в Tabletopia

![card-back-front](http://help.tabletopia.com/wp-content/uploads/2017/01/card-back-front.png)

Если у вас есть предпечатные файлы или ПнП, вам остается только отделить изображения каждого компонента в отдельные файлы.

Обратите внимание, что две стороны компонента также должны быть разными файлами.

> *Например*: Для колоды из 52 карт, вам понадобится 53 файла: 52 изображений лицевой стороны и 1 рубашка.

Двухсторонние компоненты, как карты или тайлы, должны иметь изображения одного размера.

Убедитесь, что у всех компоненты одного типа в точности совпадают размеры, вплоть до пикселя. Это важно, если вы будете использовть колоды\стопки или [Случайные элементы](http://help.tabletopia.com/knowledge-base/randomizers/). Разница даже в пиксель - критична.

> **Совет:** В статье [Как улучшить визуальный стиль игры](http://help.tabletopia.com/knowledge-base/visual-design-guide/) есть предложения по улучшению грифики игры и ее представления в Tabletopia.

![9](http://help.tabletopia.com/wp-content/uploads/2015/06/9.png)

## Соотношение см/пиксель

При адаптации реальной игры к экрану, важно сохранить пропорции размеров компонентов.

![16](http://help.tabletopia.com/wp-content/uploads/2015/06/16.png)

В Tabletopia используется теже размеры, в сантиметрах и миллиметрах. Для пересчета размеров реальных объектов, чей размер задан в сантиметрах или дюймах, в виртуальные объекты, мы должны **сконвертировать сантиметры в пиксели**

В Tabletopia **10 пикселей равны 1 миллиметру**.

>*Этот параметр подобран экспериментально при исользовании карт с большим количеством текста (например Magic: the Gathering или Берсерк). Текст остается понятным для чтения и итоговый размер карты не превышает ограничения.*

Стандартный стол, доступный в Tabletopia, обладает размерами 80&#215;120 см и может быть использован как отправная точка для определения размеров других игровых компонентов (см [Столы, поверхности и фоны](http://help.tabletopia.com/knowledge-base/tables-surfaces-and-skyboxes/)): Если вы правильно подобрали размер игрового поля и других компонентов, они будут выглядеть в точности, как реальные компоненты на реальном столе.

![15](http://help.tabletopia.com/wp-content/uploads/2015/06/15.png)
Компоненты игры "Поселенцы империи" в Tabletopia и практически тоже самое в реальной жизни.

## Масштабирование

Иногда использование пропорционых размеров больших компонентов (например [игровых полей](http://help.tabletopia.com/knowledge-base/game-board/)) приводит к увеличению размеров файла сетапа и сильное потребление ресурсов компьютера.

С такими компонентами разумнее использовть **масштабирование**, благодаря которому можно увеличить объект **до 400%**, уменьшая пропорции вплоть до **2.5 пикселей на 1 миллиметр**, и что самое главное, уменьшении файла изображения. **Использование этой возможности требуется для корректного отображения игр в браузере Chrome.**

>*Пример:* Размер игровое поле в *Septikon* было уменьшен с 8.3 до 2.65 мегабайт, увеличением масштаба JPEG изображения до 200%.
![Игровое поле Septikon](http://help.tabletopia.com/wp-content/uploads/2015/06/17.png)

**Обратное масштабирование до 50%** пригодиться если необходимо увеличить разрешение объета. Еще одно применение масштабирования - точное изменение размера объекта, если вы не хотите изменять размер оригинального изображения.

![18](http://help.tabletopia.com/wp-content/uploads/2015/06/18.png)

Пример карты в игре "Наместник" уменьшеный до 6.0 сантиметров

## Размер игровых объектов и сетапа

При принятии решении относительно размера и качества изображения компонентов учитывайте размеры файлов изображений и итоговый размер файла сетапа, который будут загружать игроки. Большие файлы приводят к увеличению времени загрузки и большему потреблению ресурсов компьютера, что может вызвать дискомфорт игроков.

### Размер объектов

**Максимально допустимый размер объекта с одной стороной - 1600&#215;1600 mm** с использованием масштабирования до 400% (или 400&#215;400 мм с масштабом 100%).

>**Совет:** Постарайтесь не превышать размер 2000&#215;2000 пикселей для каждого объекта. Производительность Tabletopia лучше, при использовании изображений меньшего размера.

**Максимальный размер файла** который вы можете загрузить - **30 MB**, но лучше стараться **не превышать 1-2 MB** для максимальной производительности.

> **Совет:** В редких случаях когда необходимы большие объекты (например гигантское игровое поле) обратитесь в [поддержку Tabletopia](mailto:support@tabletopia.com).

### Размер сетапа

**Рекомендованный размер файла сетапа - 20 MB максимум.** Следующие советы помогут вам уменьшить его:

* Качество изображений должно быть достаточное, чтобы прочитать текст или отличить одно изображение от другого, но не слишком высоким.
* Используйте одно изображение несколько раз в сетапе (напрмер рубашку для колоды карт). Изображение будет добавлено только один раз, что снизит размер сетапа.
* Уменьшите размеры больших изображений и увеличьте их масштаб в Tabletopia.
	![19](http://help.tabletopia.com/wp-content/uploads/2015/06/19.png)
* Используйте  JPEG вместо PNG, чтобы уменьшить размер картинки, если вам не нужна не прямоугльная форма объекта.
* Разделите игра на несколько сетапов, для различного количества игроков, или с различным набором компонентов. Подробнее читайте в статье [Сетапы игры](http://help.tabletopia.com/knowledge-base/game-setups/)

## Форматы файла изображения

Tabletopia поддерживает два формата изображений: .JPEG and .PNG.

### .JPEG

**Применение:**

* **Фотографические объекты.** Хорошее качество и не такой большой размер как .PNG файл.
* **Очень большие поля,** когда размер оптимизации важнее чем касество изображения.

Имейте ввиду, что в  JPEG изображения **только для прямоугольных объектов**.

**Плюсы:**

* **Размер.** Обычно размер JPEG изображения меньше, по сравнению с PNG файлом, полученным из этого же источника.

![20-1](http://help.tabletopia.com/wp-content/uploads/2015/06/20-1.png)
Размер изображения игровое поле игры Terra Mystica может быть уменьшено с 15.2 до 2.9 мегабайт при использовании JPG вместо PNG.

**Минусы:**

* **Качество.** JPEG - это метод сжатия данных цифровых изображений с потерями, поэтому такие изображения обладают ухудшеным качеством. Он не очень хорошо подходит при отображении линий, текстов и иконографики.
	![21](http://help.tabletopia.com/wp-content/uploads/2015/06/21.png)
* **Small palette bigger file size.** Note that if an image has a small number of colors in its palette, a JPEG file may have bigger size than the corresponding PNG file.
* **Rectangular shape.** JPEG files does not support alpha channel transparency, so it is not possible to create objects with round edges or a complex shape.</li>


### .PNG

PNG image files are well suited and prefered in most cases for all of the objects in the game. This format is especially useful if you want to create objects of complex shape.

**Pros:**

* **Complex shape.** The most useful application of .PNG format is to create objects of complex shape with transparent parts. One restriction still applies: There may not be transparency inside a closed image contour.

	![22](http://help.tabletopia.com/wp-content/uploads/2015/06/22.png)
	Evolution: The Origin of Species player board, opened in the graphical editor shows the broken contour of the image to allow transparency inside.

	![24](http://help.tabletopia.com/wp-content/uploads/2015/06/24.png)

	Unfortunately images which consist of several parts divided by transparent areas cannot be correctly recognized by the system. There are two possible solutions available in this case:

	1. Make the area between parts of the image non-transparent (you can try to make it of the same color as the surface or board).
	2. Consider creating several different images, each image containing only one part of the initial image. Thus you will need to combine all the parts in the setup by hand.

	Also note that the parts of the image with inner angles (e.g. the mouth area of ‘Pac-man’ style game token) support only visual transparency. Those areas act as a part of an object even if they are transparent.

* **Quality.** PNG is a lossless image file format, so your exported image will not lose quality compared to the original. Sometimes it may even be smaller than a corresponding JPEG alternative.

**Cons:**

* **Size.** In most cases the size of the PNG file is several times bigger than the JPEG file. Consider using scaling and/or JPEG files for game boards and other big objects.

## Useful Tips

<ul>
<li>**The most convenient browser** for publishing of graphic files is Opera.</li>
<li>**Make borders for the components** (especially cards) that will be taken by players into their hand. It adds a 3D look to them and helps to visually distinguish one from another.</li>
</ul>
<figure id="attachment_474" style="width: 578px" class="wp-caption aligncenter">![33](http://help.tabletopia.com/wp-content/uploads/2015/06/33.png)<figcaption class="wp-caption-text">Classic cards in Tabletopia have dark borders</figcaption></figure>
<ul>
<li id="overbright">**Don&#8217;t make components overbright.** There is a source of light in the system and some images with high initial brightness may not look good. Test your objects in the preview mode, also you may place them all on the table and review them before creating the game setup.</li>
</ul>
<figure id="attachment_1021" style="width: 569px" class="wp-caption aligncenter">![Overbright effect](http://help.tabletopia.com/wp-content/uploads/2015/11/Nations-overbright.png)<figcaption class="wp-caption-text">Yellow is very prone to being overbright.</figcaption></figure>
<ul>
<li id="dark">**Don&#8217;t make components too dark.** Special attention must be given to vertical tokens. It is ![35](http://help.tabletopia.com/wp-content/uploads/2015/06/35.png)better to increase the brightness of images used in vertical tokens.</li>
<li id="distinguishable">Make the components **easily distinguishable from one another at the mid-range distance from the table**. If you use images that are too small or images with thin lines on a similarly colored background, they may look much alike to each other even from a low camera view and the players may become confused</li>
</ul>