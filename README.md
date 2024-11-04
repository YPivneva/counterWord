Используйте модуль streams для программы простой индексации текста.
Она должна:

    Читать текстовый файл переданный в аргументах к скрипту
    Разделять входные данные на отдельные слова, разделенные разделителем (пробел, символ новой строки)
    Фильтровать не-текстовые символы (например, ',')
    Индексировать текст в вектор - массив чисел. Позиция в массиве представляет порядок всех входных слов, отсортированных в алфавитном порядке. Значение - это количество появлений определенного слова в тексте.
    Вывести результирующий вектор в файл.

Примеры:

    a c b b -> потенциальное промежуточное представление { a: 1, b: 2, c: 1 } -> [1, 2, 1]
    ab cb bss b -> [1, 1, 1, 1]
    ab, cb, bss, cb, b, cb -> [1, 1, 1, 3]
    alex, alex, juan, dima -> [2, 1, 1]

Желательно использовать потоки для всех шагов программы.