## Порівняння жадібного алгоритму та алгоритму динамічного програмування

### Результати виконання:

| Amount | Greedy Algorithm (s) | Dynamic Programming (s) |
| :----: | :------------------: | :---------------------: |
|   10   |      0.00025525      |       0.00458688        |
|   55   |      0.00030408      |       0.02503825        |
|  113   |      0.00028775      |       0.04541567        |
|  207   |      0.00021550      |       0.08200800        |
|  505   |      0.00019100      |       0.22730938        |
|  1001  |      0.00018579      |       0.48089313        |

### 1. Жадібний алгоритм

- Жадібний алгоритм вибирає монети найбільшого номіналу до повного розподілення суми.
- Кожна монета перевіряється один раз: O(n), де n — кількість монет у наборі.
- Складність залежить від швидкості розподілення суми найбільшими монетами.

### 2. Алгоритм динамічного програмування

- Цей алгоритм використовує таблицю для зберігання мінімальної кількості монет для кожної можливої суми до заданої суми.
- Ініціалізація таблиці: O(m), де m — сума для розподілу.
- Оновлення таблиці для кожної монети і суми: O(c \* m), де c — кількість монет, m — сума.
- Таким чином, загальна часова складність становить O(c \* m).

#### Висновки:

1. Жадібний алгоритм працює швидше, але не завжди дає оптимальний результат.

2. Алгоритм динамічного програмування завжди знаходить оптимальний результат, але вимагає більше часу і пам'яті.
