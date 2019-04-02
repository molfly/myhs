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