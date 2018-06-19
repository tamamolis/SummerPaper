### Welcome to my paper notes
Код к этой статье можно увидеть [здесь](https://github.com/tamamolis/VGGUnet).

##### Классы
- дороги 255 255 255
- машины 219 219 219
- деревья 132 132 132
- unlabeled 59 59 59
- трава 164 164 164
- дома 22 22 22

или, что то же самое:
- Impervious surfaces (RGB: 255, 255, 255) белый
- Building (RGB: 0, 0, 255) синий
- Low vegetation (RGB: 0, 255, 255) бирюзовый
- Tree (RGB: 0, 255, 0) зелёный
- Car (RGB: 255, 255, 0) жёлтый
- Clutter/background (RGB: 255, 0, 0) красный

##### Результаты
<p align="center">
  <img src="res/helsinki.jpg" width="350" alt="hi" class="inline"/>
  <img src="res/helsinki_result.png" width="350" alt="hi" class="inline"/>
</p>

##### Что сделано
- предобработка и кодировка изображений в удобоваримый для обучения нейросети вид (код про это можно увидеть [здесь](https://github.com/tamamolis/CreateDataForSemanticSegmentation))
- несколько моделей нейросети
  - SegNet (код [здесь](https://github.com/tamamolis/NaiveSegNet))
  - Unet (получилось так плохо, что код утерян, лучше про него не упоминать)
  - VGG + Unet (код [здесь](https://github.com/tamamolis/VGGUnet))
- модели получены, обучены, результаты есть в репозиториях, указанных выше

##### Что сделать легко и приятно
- добавить другие модели, например, VGG + Unet
- смотреть у чего лучше получается

##### Что сделать планируется и хочется, но пока не получается
- постобработка, конкретно CRF
