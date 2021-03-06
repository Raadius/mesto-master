*Проект 'Mesto'*
### [Открыть проект в браузере](https://qtrixnet.github.io/mesto/)

## Сервис по обмену фотографиями
Сервис предоставляет возможность делиться красивыми фотографиями мест в которых побывал фотограф.

Добавлен функционал живой валидации полей форм - кнопка отправки формы неактивна, если хотя бы одно из полей не проходит валидацию.

#### Основной функционал
+ Редактирование профиля
+ Добавление новой фотографии (карточку можно добавить, нажав Enter, находясь в одном из текстовых полей)
+ Удаление карточки при клике на иконку
+ Поставить / убрать лайк
+ Открытие фотографии в полном размере

#### Применен объектно-ориентированный подход разработки:
+ Использованы ES6-классы
+ Каждый класс описан в отдельном JS-файле и импортирован в index.js
+ Каждый класс выполняет строго одну задачу. Всё, что относится к решению этой задачи, находится в классе.
+ Для описания взаимодействия между классами используется слабое связывание, т.е внутри классов напрямую не создаются экземпляры других классов.
+ Экземпляр класса Card создаётся для каждой карточки.
+ Экземпляр класса FormValidator создаётся для каждой проверяемой формы.
+ Экземпляр класса UserInfo создается один раз.
+ Класс Popup имеет двух наследников, создающихся для каждого модального окна.
+ Слушатель событий, закрывающий модальное окно по нажатию на Esc, добавляется при открытии модального окна и удаляется при его закрытии.

#### Код стайл
+ Имена переменных и функций написаны в camelCase
+ Имена классов — существительные с прописной буквы
+ Имена переменных — существительные
+ Имена коллекций NodeList — существительные во множественном числе
+ Имя функции отражает то, что она делает
+ Форматирование кода - 2 пробела, например: 
```HTML
<div id="openPicture" class="popup">
  <div class="popup__fullScreen">
    <div class="popup__image-desription">
      <img class="popup__image" src="#" alt="" />
      <p class="popup__image-subtitle"></p>
      <button type="button" class="popup__close-button"></button>
    </div>
  </div>
  <div class="popup__overlay"></div>
</div>
```

#### Технологии
+ HTML5
+ CCS3
+ JavaScript (стандарт ES6)
+ ООП
+ Адаптивная верстка (мобильные устройства, планшеты, десктопы)
+ Методология БЭМ (файловая структура)
+ Flexbox
+ GRID
+ Позиционирование
+ Псевдоклассы
+ Webpack
