# Требования к дизайну
Качественный дизайн - это фундамент для завершения проекта в срок с минимальным количеством правок, а также сохранения удовольствия от работы как дизайнеров, так и разработчиков.

Приведённые ниже требования помогут в этом на все 100%:tw-1f680: 

## 1. Используй сетку
Сетка помогает организовать элементы. Как метроном в музыке, задает ритм.

![](https://habrastorage.org/webt/ch/kh/sl/chkhslnbxhbqrfhdmbewt7hxzi4.jpeg)

**Не важно какую (!)**: 12 колонок, 14 колонок, 5 линий, клетчатая сетка - главное соблюдать её, то есть соблюдать её края и отступы.

Когда сеткой начинают пользоваться и дизайнеры и разработчики — многие проблемы отпадают. Вот один из примеров [такого подхода](http://designpub.ru/%D0%BE%D1%82%D1%81%D1%82%D1%83%D0%BF%D1%8B-%D0%B2-%D0%B4%D0%B8%D0%B7%D0%B0%D0%B9%D0%BD%D0%B5-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%BD%D1%8B%D0%B9-%D0%BF%D0%BE%D0%B4%D1%85%D0%BE%D0%B4-82cad46dd34f "такого подхода").

:tw-1f517: Хорошая [статья про сетки](https://habr.com/ru/post/344910/ "статья про сетки").

## 2. Задавай текстовым блокам осознанные размеры
![](https://habrastorage.org/webt/hh/qh/fl/hhqhfl72qtx7bcir2o2jzmn24ne.jpeg)

Вот два с виду одинаковых текстовых блока. Описание и цена. Но если посмотреть как они выглядят в макете — сразу видна разница.

![](https://habrastorage.org/webt/ed/mc/fq/edmcfqachkilb2cpzorhwukkbxk.jpeg)

> **Разработчик Вася:** Когда я вижу макеты с разными отступами между блоками, меня аж трясет!!! Дизайнеры, перестаньте так делать, это же ужасно.

## 3. Следи за боковыми отступами
![](https://habrastorage.org/webt/w_/lv/_o/w_lv_objajhxlplipa9j57_kcy4.jpeg)

Разница должна быть чем-то обоснована, не должно получаться случайных значений.

> **Разработчик Вася**: Если отступы в блоке одинаковы — свойство, задающее отступ в родительском блоке, имеет вид padding: 0, 24. Во втором случае, чтобы понять закономерность отступов, придется коммуницировать с дизайнером и уточнять: что же там имелось ввиду в этом чертовом хаосе.

## 4. Используй Grow Vertically для текстовых блоков
![](https://habrastorage.org/webt/v-/f6/8n/v-f68nb8qnuetkfvru5oujnglbq.jpeg)

> **Разработчик Вася:** Хорошо когда размеры текстовых блоков по высоте изменяются автоматически. В таких блоках можно через свойства сразу получить корректную высоту. В отличии от правого примера, где высота блока 27 px, а по факту должна быть 70 px.

## 5. Соблюдай целые значения в пикселях
Расстояния между объектами должны быть выражены целыми значениями. Так же как и размеры самих объектов.

![](https://habrastorage.org/webt/xh/54/kj/xh54kjl6ige16cmevdtu-ntwkaq.jpeg)

Внешне, макеты с дробными значениями не всегда отличимы от «нормальных», но стоит погрузиться в них… и начинаются проблемы. Часто дробные значения возникают, если взять группу объектов и масштабировать ее. Очень часто такие значения свидетельствуют о том, что дизайнер поторопился и не проверил этот момент.

> **Разработчик Вася:** Вчера пришла в работу задача на верстку. Открываю макет в фигме, и что вижу… Отступы все дробные, кегель у шрифта — дробный, межстрочник — тоже дробный. Не, ну я, конечно, написал дизайнеру. Подождал ответа, подождал пока он разберется, откуда это всё взялось. В итоге только к вечеру смог приступить к этой задаче.

## 6. Используй компоненты
Идеология компонентов — главное, что отличает Figma от инструментов предыдущего поколения. Создавай компоненты по любой понятной и удобной тебе методике. Например, [концепция атомов](https://habr.com/ru/post/249223/ "концепция атомов"), при которой начиная с простейших элементов (формы, надписи) постепенно группируются более сложные компоненты на их основе.

Или [создание отдельных блоков](https://habr.com/ru/post/340774/ "создание отдельных блоков") в виде компонентов и их переиспользование. Главное, чтобы выбранный подход был логичным и понятным для тех, кто будет работать после или одновременно с тобой. Мы, как правило, используем компоненты в зависимости от сложности проекта.

![](https://habrastorage.org/webt/kk/zw/8n/kkzw8niykuycpe-mkkeptihghks.jpeg)

Компонентам и их использованию посвящены отдельные статьи. С описанием работы constraints и сеток внутри компонентов.

## 7. Называй группы и фреймы осмысленно
Понятные названия помогут другим разобраться в твоем макете и не вспоминать тебя“теплыми”словами.

![](https://habrastorage.org/webt/or/9o/is/or9ois-khyfhxsnvvt7-xqjsp4w.jpeg)

> **Разработчик Вася:** Среди разработчиков есть культура написания имен переменных и функций. А вы, дизайнеры, чем лучше? Почему вы с легкостью отдаете макеты с неинформативными названиями? Подписывайте ясно и четко названия фреймов и компонентов.

## 8. Делай растр с двукратным или трехкратным запасом по размеру
Существует много мониторов с увеличенной плотностью пикселей. Что это означает для дизайнера?

При одинаковых физических размерах экранов на каждом из них помещается разное количество пикселей. И если подготовить растровое изображение для обычного монитора 1:1, то на ретине оно будет выглядеть размытым.

![](https://habrastorage.org/webt/ze/kp/ad/zekpadel0eaxb8nhzj2xdxie6ea.jpeg)

> **Разработчик Вася:** Помню как в 2000-м году выходил в интернет через старый добрый US Robotics Courier на скорости 14 400 бит/с… Тогда графику делали 1в1, сайты верстали таблицами, не было ретин и прочих смартфонов. В общем жили не тужили. Сейчас CSS псевдо классы позволяют ребятам с ретиной и прочими hi-end дисплеями подгружать специально для них предназначенные растровые изображения. При этом не грузить их всем остальным.
