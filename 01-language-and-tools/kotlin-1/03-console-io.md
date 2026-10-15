# Консольный ввод и вывод

[← Типы данных](02-data-types.md) · [Этап 1](../README.md) · [Главная](../../README.md) · [Операции с числами →](04-number-operations.md)

## Коротко

Как программа общается с пользователем через консоль: `print` и `println` выводят текст, `readLine` и `readln` читают то, что ввел пользователь. Ввод всегда приходит строкой.

## Вывод

- print() - выводит значение и остается на той же строке
- println() - выводит значение и переводит курсор на новую строку

```kotlin
print("Hello ")
print("Kotlin")
println()            // без аргументов просто переводит на новую строку
println("Kotlin is fun")
```

Вывод:
```
Hello Kotlin
Kotlin is fun
```

## Ввод

Ввод с клавиатуры читается функцией readLine(), она возвращает введенную строку
```kotlin
print("Введите имя: ")
val name = readLine()
println("Ваше имя: $name")
```

Вывод:
```
Введите имя: Lyoha
Ваше имя: Lyoha
```

Можно читать несколько значений подряд, каждый вызов readLine() ждет одну строку
```kotlin
print("Введите имя: ")
val name = readLine()
print("Введите email: ")
val email = readLine()

println("Ваше имя: $name")
println("Ваш email: $email")
```

> [!NOTE]
> readLine() - возвращает String?, потому что строка может оказаться null
>
> В новых версиях Kotlin есть readln() - она возвращает обычный String, поэтому ей пользоваться проще

```kotlin
val name: String? = readLine()   // String? - может быть null
val city: String = readln()      // String - всегда строка
```

> Ввод всегда приходит строкой, даже если пользователь ввел число. Чтобы получить число, строку надо преобразовать

---

[← Типы данных](02-data-types.md) · [Этап 1](../README.md) · [Главная](../../README.md) · [Операции с числами →](04-number-operations.md)
