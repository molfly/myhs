# Haskell

## Урок 1
### Интерпретатор
> ghci

[Ссылка на уроки](https://youtu.be/I5UUkmy-I9I).  
[Скачать тут](https://www.haskell.org/platform/mac.html).

Запуск после установки 

```
$ ghci
GHCi, version 8.6.3: http://www.haskell.org/ghc/  :? for help
Prelude>
```

Все команты интерпретатора начинаются с двоеточия ```:```

Вот компиляция модуля и исполнение функции:
```
Prelude> :load Test
[1 of 1] Compiling Test             ( Test.hs, interpreted )
Ok, one module loaded.
*Test> sayHello
Hello from module Test!
```

### Команды:

загрузить модуль `:load` или `:l`  
перезагрузить модуль `:reload` или `:r`  
выйти `:quit` или `:q`  

### Табы и пробелы
Одна табуляция равна 8 пробелам.

## Механизм вызова функций и роль скобок

Вызов функции не требует заключения в скопки. Смысл скобок математический - порядок действий.

```
Prelude> acos (cos pi)
3.141592653589793
Prelude> max 5 42
42
```

### Частичное применение функции
Частичное применение функции. При n переменных. Функция одной переменной, возвращающая нам функцию n-1 переменной.

### Объявление функции 
+ задать имя
+ указать параметры
+ поставить знак равенства
+ реализовать тело функции

Имя функции и имена параметров должны начинаться с буквы в нижнем регистре.

Пример функции описан в `demo.hs` [↳](https://github.com/molfly/myhs/blob/master/step1/demo.hs).

Вызов
```
$ ghci
GHCi, version 8.6.3: http://www.haskell.org/ghc/  :? for help
Prelude> :l Demo
[1 of 1] Compiling Main             ( Demo.hs, interpreted )
Ok, one module loaded.
*Main> sumSquares 1 2
5
```