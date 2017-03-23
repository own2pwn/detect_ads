# Лукьянов Илья, ПМИ-151 #

## Анализ видеопоследовательностей для автоматического поиска и выделения рекламы ##

Собственно, название отлично отражает цель проекта: автоматическое выделение рекламы.

### Актуальность задачи ###

* Существуют различные решения для автоматического поиска и удаления рекламных вставок из видеопотока, у всех есть свои преимущества и недостатки.
* Хотелось бы реализовать работающую с хорошей точностью утилиту для поиска рекламы, желательно работающую в реалтайме или с небольшой буферизацией, сохраняющее очищенный видеопоток "на лету".

### Цели ###

* Научиться работать с библиотекой OpenCV для анализа видео.
* Научиться работать с различными алгоритмами поиска особых точек, дескрипторами, алгоритмами кластеризации и поиска.
* 

### Используемые технологии ###

* Python — язык, с которым я себя комфортно чувствую, к тому же являющийся более или менее стандартом (вместе с C++) в анализе видео и изображений.
* OpenCV — одна из лучших библиотек компьютерного зрения.
* ffmpeg — пожалуй, лучшая утилита для обработки видео.
* STIP — отличный алгоритм поиска точек интереса в пространстве-времени видео. 
* Optical Flow
* Различные библиотеки для анализа данных для Python.
* Другие алгоритмы для обработки видео (будут заполнены по мере использования в проекте)

### Архитектура ###

Тут будет картинка.

### Как запустить ###

* Требуется установленный OpenCV 2 (для работы STIP). Возможно, будет в репозитории, если не будет проблем с зависимостями.
* Требуется OpenCV 3 (любой подойдёт, главное чтоб были биндинги для Python)
* Требуется ffmpeg и pyav (самый простой способ установить — через conda: `conda install av -c conda-forge`)

Когда более или менее закончу добавлять зависимости, разверну на чистой виртуалке с Ubuntu 16.04 и напишу подробную инструкцию для неё.

### Описание функциональности ###



### План работы ###

* Интерфейс для работы со STIP из Python — сделано
* Кластеризация найденных особых точек — сделано
* Поиск предварительно выбранного видео в потоке — сделано
* Поиск сцен при помощи Optical Flow — сделано
* Сохранение видеопотока без рекламы — практически сделано
* Поиск повторяющихся сцен и составление базы — в процессе