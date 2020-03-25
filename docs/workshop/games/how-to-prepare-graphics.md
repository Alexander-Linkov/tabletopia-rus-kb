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

**Maximum size of one continuous one-sided object** in the system is **1600&#215;1600 mm** using the scaling maxed to 400% (or 400&#215;400 mm with scaling set at 100%).
**Tip:** Try not to exceed the image size of 2000&#215;2000 pixels for each object. The system performance is better when the size is lesser.
**Maximum file size** you can upload is **30 MB**, but you should try to keep it **not more than 1-2 MB** for the optimal performance.
**Tip:** In a rare situation when you need a bigger object (e.g. gigantic game board) contact [Tabletopia’s Support](mailto:support@tabletopia.com). We will help you to find the optimal solution to this problem if it is possible.
### Setup Size
**Recommended setup file size is max 20 MB.** The following recomendations will help you reduce the size of your setup:
<ul>
<li>The quality of images should be good enough to read from and discern one image from another, but not too high.</li>
<li>Use the same image several times in the setup (e.g. back image of the deck of cards), it will be added only once and the size will be adjusted accordingly.</li>
<li>![19](http://help.tabletopia.com/wp-content/uploads/2015/06/19.png)Decrease the size in pixels of the big images and scale them up by editing the settings of each image in Tabletopia’s system.</li>
<li>Use JPEG images instead of PNG to decrease the size of the image when you do not need to set a complex shape.</li>
<li>Split the game to several setups for different number of players or for different sets of components, see [Game Setups](http://help.tabletopia.com/knowledge-base/game-setups/) for details.</li>
</ul>
## Image File Formats
Tabletopia allows two different image file formats to be used in the game: .JPEG and .PNG.
### 
**Uses:**
<ul>
<li>**Photographic images.** The quality of the image is quite good and the size of the file is not as big as PNG.</li>
<li>**Very large game boards,** when the size optimization is more important than the quality of the image.</li>
</ul>
Note that you can use JPEG images for **rectangular** **objects** only.
**Pros:**
<ul>
<li>**Size.** Generally the size of a JPEG image is lower than the size of a corresponding PNG image, exported from the same source.</li>
</ul>
<figure id="attachment_459" style="width: 1000px" class="wp-caption alignnone">![20-1](http://help.tabletopia.com/wp-content/uploads/2015/06/20-1.png)<figcaption class="wp-caption-text">Terra Mystica’s game board may be shrunk in size from 15.2 down to 2.9 megabytes by using JPG instead of PNG.</figcaption></figure>
**<br />
Cons:**
<ul>
<li>**![21](http://help.tabletopia.com/wp-content/uploads/2015/06/21.png)<strong>Quality.** </strong>JPEG is a method of lossy compression for digital images, so it provides less quality. It is not well suited for line drawings and other textual or iconic graphics.</li>
<li>**Small palette bigger file size.** Note that if an image has a small number of colors in its palette, a JPEG file may have bigger size than the corresponding PNG file.</li>
<li>**Rectangular shape.** JPEG files does not support alpha channel transparency, so it is not possible to create objects with round edges or a complex shape.</li>
</ul>
### 
PNG image files are well suited and prefered in most cases for all of the objects in the game. This format is especially useful if you want to create objects of complex shape.
**Pros:**
<ul>
<li>**Complex shape.** The most useful application of .PNG format is to create objects of complex shape with transparent parts. One restriction still applies: There may not be transparency inside a closed image contour.</li>
</ul>
<figure id="attachment_463" style="width: 1016px" class="wp-caption aligncenter">![22](http://help.tabletopia.com/wp-content/uploads/2015/06/22.png)<figcaption class="wp-caption-text">Evolution: The Origin of Species player board, opened in the graphical editor shows the broken contour of the image to allow transparency inside.</figcaption></figure>
![24](http://help.tabletopia.com/wp-content/uploads/2015/06/24.png)Unfortunately images which consist of several parts divided by transparent areas cannot be correctly recognized by the system. There are two possible solutions available in this case:
<ol>
<li>Make the area between parts of the image non-transparent (you can try to make it of the same color as the surface or board).</li>
<li>Consider creating several different images, each image containing only one part of the initial image. Thus you will need to combine all the parts in the setup by hand.</li>
</ol>
Also note that the parts of the image with inner angles (e.g. the mouth area of ‘Pac-man’ style game token) support only visual transparency. Those areas act as a part of an object even if they are transparent.
<ul>
<li>**Quality.** PNG is a lossless image file format, so your exported image will not lose quality compared to the original. Sometimes it may even be smaller than a corresponding JPEG alternative.</li>
</ul>
**Cons:**
<ul>
<li>**Size.** In most cases the size of the PNG file is several times bigger than the JPEG file. Consider using scaling and/or JPEG files for game boards and other big objects.</li>
</ul>
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