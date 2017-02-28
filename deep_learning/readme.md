# Краткое описание статей:

### Imagenet classification with deep convolutional neural networks

Одна из классических статей, с которых начался современный виток диплернинга.

Появление ImageNet позволило решать задачу классификации изображений на
качественно новом уровне.

Авторы использовали сверточную сеть из 8 слоев: 5 сверточных, 3 полносвязных,
последний слой - softmax на 1000 классов.

Обучали на двух GPU GTX 580 (по 3Gb памяти) в течении 6 дней.

Функция активации: ReLU

Функция потерь: множественная логистическая регрессия.

Так же использовали локальную нормализацию (local normalization).

Для борьбы с оверфитом применили аугментации и дропаут.

Полученные результаты:
- ошибка на top-1: 35.7%
- ошибка на top-5: 17.0%

<hr />

### Using Deep Learning and Google Street View to Estimate the Demographic Makeup of the US

Исследовали использовали снимки с Google Street View, локализовали автомобили,
с помощью сверточных сетей определили марку, модель и год выпуска авто и на основе этого получали демографические данные по району: национальность, образование, доход, за кого голосуют.

*For instance, if the number of sedans encountered during a 15-minute drive through a city is higher than the number
of pickup trucks, the city is likely to vote for a Democrat during the next Presidential
election (88% chance); otherwise, it is likely to vote Republican (82%).*

<hr />
