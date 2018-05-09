# Editor-3D-CAD
HTML 3d animation design editor

Данное web-приложение задумывалось для создания 3D анимации с применением технологии webgl (three.js) в рамках HTML5

Demo: https://sozercaniekosmosa.github.io/Editor-3D-CAD/

Приложение не претендует на лавры профессионального инструмаента и создавалось скорее для развития навыков создания подобных приложений, хотя изначально планировалось сделать некоторый коммерческий уклон.

![скриншот](https://github.com/sozercaniekosmosa/Editor-3D-CAD/blob/master/pic/3dcad-2.png)

## Возможности:

### Общие:
  - Undo
  - Redo

### Операции над объектами:
  - Параллельный перенос          (W)
  - Поворот                       (E)
  - Масштабирование               (R)
  - Операции над опорной точкой
  - Переключение м/у системами голабльная/локальная
  - Создание/удаление связей (родительский -> дочерний)
  - Grid snap
  - Angel snap
  - Центрование по выделенному    (shift+F)

### Навигация/отображение работа с камерой:
  - shift+drag + right mouse buttom -> pan
  - shift+drag + left mouse buttom  -> rotate 
  - shift+drag + wheel              -> zoom
  - Переключение камеры орбитальная/свободная

### Свет:
  - Интенсивность                 (L)
  - Дистанция                     (D)
  - Цвет
  
### Узловая анимация:
Позволяет анимировать объекты по ключевым кадрам линейно интерполируя координаты, угловые отношения и некоторые другие параметры м/у объектами.
### Анимация имеет ряд инструментов:
  - Добавление ключевых кадров
  - Изменение количества точек интерполяции на кадый ключевой кадр
  - Запуск/останов анимации
  - Рендеринг (кадый кадр анимации сохраняется в отдельном файле)

### Среда разработки:
  - webstorm
  
### Примечание:
  - Для запуска используйте index.html
  - На объекты может накладываться заранее подготовленная текстура, но GUI для этого нет.
  - Так же отсутствует GUI для добавления новых 3D объектов, но программная реализация таких возможностей
    присутствует в виде методов.
  - Для использования текстур необходим запуск с сервера, данное ограничение накладывается спецификацией webgl.
  - Данное приложение тестировалось под FF и Chrome (под IE10 не работает)
