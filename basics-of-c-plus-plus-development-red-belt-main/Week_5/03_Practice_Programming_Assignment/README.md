## Оператор присваивания для SimpleVector ##

### Условие ###

В видеолекции мы с вами познакомились с конструктором копирования и оператором присваивания, а также написали конструктор копирования для SimpleVector. В этой задаче вам нужно реализовать оператор присваивания для SimpleVector.

Напомним, что следующий код вызывает **конструктор копирования**:

```cpp
SimpleVector<int> source(5);
SimpleVector<int> dest = source; // Конструктор копирования
```

А код ниже — **оператор присваивания**:

```cpp
SimpleVector<int> source(5);
SimpleVector<int> dest;
dest = source; // Оператор присваивания
```

Наличие такого синонима позволяет записать возвращаемый тип функции GroupHeavyString в виде vector<Group<String>>, что читается понятнее, чем vector<vector<String>>.

Слова в каждой группе должны располагаться в том же порядке, что и в исходном наборе. При этом порядок самих групп значения не имеет.

Строка типа String не обязана состоять из символов типа char. Тип символа можно получить с помощью выражения typename String::value_type или Char<String>, если определить соответствующий синоним:

```cpp
template <typename String>
using Char = typename String::value_type;
```

Вам дан cpp-файл, который подключает заголовочный файл simple_vector.h и содержит небольшой набор юнит-тестов. Пришлите на проверку файл simple_vector.h с реализацией оператора присваивания.

### Файл с заготовкой решения ###

[simple_vector_copy_assignment.cpp](Source/simple_vector_copy_assignment.cpp)


# [Решение](Solution/simple_vector_copy_assignment.cpp)
