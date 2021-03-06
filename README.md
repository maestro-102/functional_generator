# functional_generator | функциональный генератор

В один прекрасный момент, когда сидел за ремонтом автомобильного усилителя, я понял, что у меня до сих пор нет такой крутой штуки как генератор сигналов. По сути мне нужно было просто подать на вход устройства какую-нибудь синусоиду, чтобы вернуть его к полноценной жизни. Поэтому мне, в принципе, было без разницы откуда его взять. Исходя из этого и был собран простейший функциональный генератор на базе Arduino.

Содержание
---
1. <a href="https://github.com/maestro-102/functional_generator#%D1%84%D0%BE%D1%82%D0%BE%D0%B3%D1%80%D0%B0%D1%84%D0%B8%D0%B8">Фотографии</a>
2. <a href="https://github.com/maestro-102/functional_generator#%D1%85%D0%B0%D1%80%D0%B0%D0%BA%D1%82%D0%B5%D1%80%D0%B8%D1%81%D1%82%D0%B8%D0%BA%D0%B8">Характеристики</a>
3. <a href="https://github.com/maestro-102/functional_generator#%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5">Описание</a>
4. <a href="https://github.com/maestro-102/functional_generator#%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D1%8B-%D0%B4%D0%BB%D1%8F-%D0%BF%D1%80%D0%BE%D1%81%D0%BC%D0%BE%D1%82%D1%80%D0%B0-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2">Программы для просмотра файлов</a>
5. <a href="https://github.com/maestro-102/functional_generator#%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B0-%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0">Структура проекта</a>

Фотографии
---
<a href="https://github.com/maestro-102/functional_generator/blob/master/images/1.jpg" target="_blank">
    <img src="https://github.com/maestro-102/functional_generator/blob/master/images/1.jpg?raw=true" width=30% alt="preview">
</a>

<a href="https://github.com/maestro-102/functional_generator/blob/master/images/2.jpg" target="_blank">
    <img src="https://github.com/maestro-102/functional_generator/blob/master/images/2.jpg?raw=true" width=30% alt="preview">
</a>

<a href="https://github.com/maestro-102/functional_generator/blob/master/images/3.jpg" target="_blank">
    <img src="https://github.com/maestro-102/functional_generator/blob/master/images/3.jpg?raw=true" width=30% alt="preview">
</a>

Характеристики
----
- цифровое программирование частоты и фазы.
- потребляемая мощность 12.65 мВт при напряжении 3 В.
- диапазон выходных частот от 0 МГц до 12.5 МГц.
- разрешение 28 бит (0.1 Гц при частоте опорного сигнала 25 МГц).
- тип сигнала: синусоидальные, треугольные и прямоугольные выходные колебания.
- напряжение питания от 2.3 В до 5.5 В.


Описание
---
База устройства - Arduino UNO. Генератор сделан в виде шилда. Т.е., когда нужен генератор, берем этот шилд, вешаем на Arduino UNO, прошиваем и работаем. Когда генератор не нужен, Arduino можно использовать для других целей: экспериментов, отлаживания прошивок, и т.д. Сердце генератора - сам генератор AD9833, заказанный на всемирной площадке... 

Программы для просмотра файлов
-----
1. Sprint Layout 6.0 - для проектирования печатных плат \
Расширение: \*.lay6 \
Ссылка: https://radioaktiv.ru/loads/softf/pcb/27881-sprint-layout-60-rus.html

2. Splan 7.0 - для черчения электрических схем \
Расширение: \*.spl7 \
Ссылка: http://splansoft.ru/

Структура проекта
-----------------

Описание файловой структуры проекта:

    functional_generator
    ├── sketch         - папка программным обеспечением
    ├── image          - папка с фотографиями устройства
    ├── pcb            - печатная плата
    ├── shemas         - схема устройства
    └── README.md          
