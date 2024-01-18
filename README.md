# Обнаружение объектов в реальном времени с использованием MobileNet SSD

Этот проект демонстрирует обнаружение объектов в реальном времени с использованием сети MobileNet Single Shot Multibox Detector (SSD) и OpenCV. Программа захватывает видео с источника камеры и наложит рамки вокруг обнаруженных объектов, а также отобразит метки классов и уверенность.

## Использование

Для запуска обнаружения объектов в реальном времени используйте следующую команду:

```bash
python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
Убедитесь, что вы заменили MobileNetSSD_deploy.prototxt.txt и MobileNetSSD_deploy.caffemodel путями к вашему файлу 'deploy' prototxt и предварительно обученной модели.

Зависимости
imutils
numpy
OpenCV
Установите зависимости с помощью следующей команды:

bash
Copy code
pip install imutils numpy opencv-python
Настройка
Измените уровень уверенности для слабых обнаружений, изменив аргумент -c или --confidence. По умолчанию установлено значение 0.2.

Сохранение обнаруженных объектов
Обнаруженные объекты можно сохранить в указанную папку. Папка по умолчанию установлена как detected_objects. Обновите переменную output_folder в скрипте, чтобы изменить место сохранения.

Лицензия
Этот проект лицензирован в соответствии с лицензией MIT - см. файл LICENSE.md для получения подробной информации.

Благодарности
Модель MobileNet SSD была обучена командой OpenCV и может быть найдена здесь.
Отдельное спасибо разработчикам imutils за упрощение видеопотока и расчета кадров в секунду.
Не стесняйтесь вносить свой вклад или сообщать об ошибках!
