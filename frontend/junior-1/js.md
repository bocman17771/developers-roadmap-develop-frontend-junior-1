# JavaScript

### Данные

* Какие типы данных есть в JS?
* Какие типы в JS изменяемые, а какие нет?
* Что значит ссылка на переменную?
* Что такое `NaN`? Как проверить, что переменная - `NaN`?
* Что значит создавать переменную через конструктор или через литерал?
* Когда при обращении к свойству объекта стоит использовать точечную нотацию, а когда через строку в квадратных скобках?
* Что произойдет, если попытаться получить несуществующее в объекте свойство?
* Что делает `hasOwnProperty`?
* Когда использовать `null`, а когда `undefined`?
* Какие есть способы создания глобальных переменных?
* Для чего нужна директива `use strict`?

### Выражения

* Что такое выражения и инструкции? В чем отличия между ними?
* Чем отличаются `var`, `let` и `const`?  
  Почему использование `const` может быть предпочтительнее?
* Что такое тернарный оператор?
* Что делает оператор `for..in`? Какие имеются особенности при использовании этого оператора с массивами?
* Как безопасно проверить, что переменная существует (была объявлена), и не словить ReferenceError?

### Массивы

* Способы создания массивов:
  * литерал
  * конструктор
  * `Array.from()`
  * `Array.of()`
* Какие есть способы удалить элемент из массива и в чем их особенности?
* Свойство `length` у массива
  * Какое значение будет свойства `length` у массива и почему:  
    ```javascript
    const a = [1, 2, 3];
    a[10] = 4;
    ```
  * Что будет, если переприсвоить новое значение?
  * Влияет ли на `length` удаление элемента посередине массива?  
    Какие способы удаления элементов влияют на длину, а какие нет?
* Как проверить, что в переменной лежит массив?
* Что делают, как и когда использовать следующие методы:
  * `reduce`
  * `sort`
  * `filter`
  * `map`
  * `forEach`
  * `some`
  * `every`

### Функции

* Какие есть 4 шаблона вызова функции, которые задают контекст выполнения этой функции?
  * Как директива `use strict` влияет на `this` внутри функции?
* Каков наиболее простой паттерн, позволяющий облегчить читаемость функции, когда у нее огромное количество аргументов?
* Как получить все аргументы функции, включая те, что не объявлены, но все-таки были переданы?
* Что такое рекурсия? Когда удобно ее использовать?
* Что такое замыкания и в каких случаях они могут быть полезны?
  Как сохранить состояние с помощью замыкания, и для чего это состояние может быть использовано?
* Решить такую вот проблему: пускай у нас есть массив ссылок, и наша задача — сделать так, чтобы при клике на каждую выводился `alert`'ом ее порядковый номер. Первое решение, что приходит в голову, выглядит так:  
  ```javascript
  for (var i = 0; i < links.length; i++) {
    links[i].onclick = function() {
      alert(i);
    }
  }
  ```  
  На деле же оказывается, что при клике на любую ссылку выводится одно и то же число — значение `links.length`.  
  Почему так происходит и как это исправить?
* Что такое callback (функция обратного вызова)?  
  Когда они обычно применяются?

### Прототипы

* Что такое функция-конструктор?  
  Как их создавать и как ими пользоваться?
* Что такое прототип? Какие возможности имеет/дает?
* Почему методы объекта лучше хранить в прототипе, а не в самом объекте?
* Можно ли создать инстанс функции через конструктор? 
* Как создать объект, который ни от чего не наследуется?
* Какие есть способы отнаследоваться в JavaScript? _(Как минимум 3)_  
  В чем их отличия и нюансы?
* Как в переопределенном методе у наследующего класса вызвать переопределяемый метод родительского?  
  Пример псевдокода:  
  ```javascript
  class Person
    method getFullName()
      return this.name + this.surname

  class Employee extends Person
    method getFullName()
      return super() + this.position
  ```


#### Ресурсы

* [Types (Airbnb JavaScript Style Guide)](https://github.com/airbnb/javascript#types)
* [Объекты как ассоциативные массивы](https://learn.javascript.ru/object)
* [Выражения и инструкции](https://ru.hexlet.io/courses/introduction_to_programming/lessons/expressions/theory_unit)
* [JavaScript: Выражения и инструкции](https://puzzleweb.ru/javascript/2_syntax3.php)
* [Variable Declarations](https://www.typescriptlang.org/docs/handbook/variable-declarations.html)
* [Массивы. MDN](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array)
* [Some Closure on Closures](https://dev.to/jckuhl/some-closure-on-closures-44ga)
* [What's so useful about closures (in JS)?](https://softwareengineering.stackexchange.com/questions/203507/whats-so-useful-about-closures-in-js)
* [Why would a program use a closure?](https://softwareengineering.stackexchange.com/questions/285941/why-would-a-program-use-a-closure)
* [Четыре паттерна вызова функций в JavaScript](https://habr.com/ru/post/155815/)
* [Каррирование функций в JavaScript](https://habr.com/ru/company/ruvds/blog/427295/)
* [Карринг и частичное применение](https://www.ibm.com/developerworks/ru/library/j-jn9/)
* [Мемоизация в JS и ускорение функций](https://habr.com/ru/company/ruvds/blog/332384/)
* [ES6 классы](http://jsraccoon.ru/es6-classes)
* [Классы в ECMAScript 6](https://frontender.info/es6-classes-final/)
* [Замыкание](https://habr.com/ru/company/ruvds/blog/513764/)
