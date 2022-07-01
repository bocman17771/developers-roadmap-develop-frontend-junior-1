# HTML

* HTML5, как сделать верстку семантичной и зачем это нужно?
* Что такое `doctype` и зачем он нужен?
* Какие есть отличия у тегов `div`, `p`, `span`, `a`?
* Что такое инлайновые элементы (например, `b`, `i`, `strong`, `em`)?
* Как создавать таблицы в html?
  * `border-spacing`, `border-collapse`
  * `colspan`, `rowspan`
  * `table-layout`
  * `caption`
  * `scope`
  * `display: table`, `table-cell`, `table-row` и т.д.
* В чем заключаются отличие чекбокса от радио кнопок?  
  Как связать радиокнопки в группу?
* Что такое тег `<label>` и как с ним работать?
* БЭМ:
  * Что это такое и в чем его польза?
  * Блок
    * Что такое, когда следует создавать?
    * Может ли блок содержать другие блоки?
    * Почему не стоит задавать внешнюю геометрию блокам?
  * Элемент
    * Что такое, когда следует создавать?
    * Может ли элемент содержать другие элементы?
    * Может ли элемент содержать блоки (блок, к которому он относится, или другие блоки)?
    * Можно ли создавать элемент элемента?
    * Может ли элемент использоваться вне блока?
    * Может ли существовать блок без элементов?
  * Модификатор
    * Что такое, когда следует использовать?
    * Когда следует использовать булевый модификатор, а когда модификатор ключ-значение?
  * Является ли корректным следующий код?  
    ```html
    <div class="button__red"> Click me </div>
    ```
  * Почему в CSS по БЭМ не рекомендуется использовать селекторы по id и по тегам?
  * Как препроцессоры помогают избежать неудобств с дублированием названий в коде?
  * Какие альтернативы есть БЭМ _(хотя бы 2)_ и в чем их плюсы и минусы?
  * Что такое миксы в БЭМе?  
    Какие особенности работы с ними есть?
  * Как бы вы отрефакторили данный код:  
    ```html
    <header class="header">
      <img class="logo">
      <form class="search-form">
        <input type="input"/>
        <button type="button"></button>
      </form>
      <ul class="lang-switcher">
        <li class="lang-item">
          <a class="lang-link" href="url">en</a>
        </li>
        <li class="lang-item">
          <a class="lang-link" href="url">ru</a>
        </li>
      </ul>
    </header>
    ```
* Зачем нужны метатеги?
* Что такое data-атрибуты?  
  Когда они могут быть полезны?
* Как стилизовать `svg`? Какие основные атрибуты и CSS-свойства используются для этого?
* Что такое специальные html-сущности (неразрывный пробел, длинное тире) и как с ними работать?


#### Ресурсы

* [Людоедский интерфейс, Вадим Макеев](https://www.youtube.com/watch?v=ssJsjGZE2sc)
* [HTML Academy](https://htmlacademy.ru/)
* [HTML (MDN)](https://developer.mozilla.org/ru/docs/Web/HTML)
* [HTML и HTML5. Описание тегов по основным разделам](https://html5book.ru/html-html5/)
* [Основы методологии БЭМ](https://ru.bem.info/methodology/quick-start/)
* [Альтернативы БЭМ](https://habr.com/ru/post/256109/);
* [SVG: заливка и обводка](http://css.yoksel.ru/svg-fill-and-stroke/)
* [Способы организации CSS-кода](https://habr.com/ru/post/256109/)