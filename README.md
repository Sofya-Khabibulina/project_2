# Проект "Генератор QR-кода"
*Подготовлен:*

Хабибулина Софья Аркадьевна (467896)

Лессик Софья Романовна (466503)

## **Распределение обязанностей:**

Хабибулина Софья —

Лессик Софья —

---
## Описание проекта:

Создание и кастомизация QR-кода с возможностью выбора формы, цвета самого QR-кода и цвета его фона (из предложенных). Также пользователь сможет ввести текст (например, поздравление), который увидит после сканирования, и вставить URL картинки для фона QR-кода. Благодаря этим функциям получается уникальный QR-код, который можно использовать для самых разных целей, в зависимости от дизайна.

*Примечание 1:*

При создании проекта мы опирались на предыдущий (https://github.com/Sofya-Khabibulina/project_1), а также использовали информацию по этим ссылкам:

- https://realpython.com/python-generate-qr-code/

- https://pydocs.ru/python-qr-code/

Также нами использовались нейросети (одна из ним: Марти GPT) для обнаружения ошибок в коде.

---
## Пример использования

$ python main.py

Введите текст для QR-кода, который вы увидите после сканирования:

> С Новым годом!

Выберите форму QR-кода (square, circle, rounded_square):

> circ

Ошибка: форма не распознана. Пожалуйста, выберите из доступных.

Выберите форму QR-кода (square, circle, rounded_square):

> circle

Доступные цвета:  red, blue, green, yellow, orange, purple, cyan, magenta, pink, teal, white, black

Введите цвет заливки (пикселей) для QR-кода: 

> purp

Ошибка: Недопустимый цвет: purp. Доступные цвета: red, blue, green, yellow, orange, purple, cyan, magenta, pink, teal, white, black

Введите цвет заливки (пикселей) для QR-кода:

> purple

Доступные цвета:  red, blue, green, yellow, orange, purple, cyan, magenta, pink, teal, white, black

Введите цвет фона для QR-кода:

> pink

QR-код успешно сгенерирован.

Введите URL для изображения фона: 

> /

Недопустимый URL. Он должен начинаться с http:// или https://.

Введите URL для изображения фона: 

> https://i.pinimg.com/736x/61/5d/5d/615d5d479f4a3a997de658cd04e5029d.jpg

QR-код с цветом и формой успешно сохранен как 'final_qrcode.png'.

![image](https://github.com/user-attachments/assets/fd31a077-4a70-42a0-a4b4-69b1a89a25d2)


---

*Примечание 2:*

Если были выбраны слишком светлые/слишком яркие или недостаточно контрастные цвета, телефон не всегда сможет считать QR-код. Это относится и к сочетанию цвета картинки на фоне и цветов QR-кода. Ответственность за подбор цветов, такой, чтобы код считывался, лежит на пользователе. Если код используется ради эксперимента, то вариации цветов могут быть самыми разными, тут все зависит от вашей креативности :)
