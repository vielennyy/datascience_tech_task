# datascience_tech_task
A technical task for a Data Science Camp

Завдання 1: Написати програму розв’язування систем 3 лінійних рівнянь з 3 невідомими, та вказати
розв’язок X системи AX= B, де
    1 2 3       1
A = 0 1 2   B = 1
    2 0 0       0
Формат відповіді:
● Розв’язок системи XT = (? ? ?)
(замінити ‘?’ відповідними значеннями)
● Код програми, котра приймає інші значення матриць A і B

Завдання 2: Написати програму, котра приймає на вхід матрицю зі значеннями 1 або 0 (живий або
мертвий стани) та ітеративно замінює значення в матриці за наступними правилами:
● якщо в живої клітини два чи три живих сусіди, то вона лишається жити;
● якщо в живої клітини один чи немає живих сусідів, то вона помирає від «самотності»;
● якщо в живої клітини чотири та більше живих сусідів, то вона помирає від «перенаселення»;
● якщо в мертвої клітини рівно три живих сусіди, то вона оживає.
Кожна клітинка має вісім сусідів.
Формат відповіді:
● Код програми, котра виводить 7-му ітерацію наступного початкового стану:
[[1,0,0,0,0,0,0],
[0,0,1,0,0,1,1],
[1,0,0,1,0,0,1],
[0,1,1,0,1,1,0],
[1,1,1,1,0,0,1],
[1,1,1,1,1,1,1],
[1,1,0,1,1,0,1]]

Завдання 2.1*: Модифікувати програму так, щоб вона випадково генерувала початковий стан матриці з
заданим розміром і мала можливість безкінечно симулювати ітерації.

Завдання 2.2**: Візуалізувати симуляцію ітерацій (matplotlib / seaborn / plotly / etc).

Завдання 3: Ймовірність випадання сторони ‘H’ для кожної з 5 монет (назвемо їх m1, m2, m3, m4, m5) зі
зміщеним центром ваги рівна відповідно [0.1, 0.2, 0.4, 0.8, 0.9]. З монет навмання вибрали одну і почали
випробування. Визначити ймовірність випадання ‘H в наступному випробуванні після кожного з 8
фактично проведених випробувань:
[H H H T H T H H] (тут ‘T’ протилежна сторона монети).
Наприклад, до першого випробування ймовірність випадання ‘H’ рівна ~0.48 (за формулою повної
ймовірності, з урахуванням рівноможливості вибрати кожну монету з наявних). Після випадання ‘H’ в
першому випробуванні, ймовірності гіпотез, що вибрана монета є m1/m2/m3 зменшились, а відповідно
ймовірності гіпотез, що вибрана монета m4/m5 збільшились а, отже і змінилась ймовірність випадання ‘H’
в наступному (другому) випробуванні і стала рівною ~0.69. Аналогічно після випадання ‘H’ в другому
випробування треба переоцінити ймовірність випадання ‘H’ в третьому, і т.д.
Формат відповіді:
● список ймовірностей з точністю до сотих [ 0.69, ?, ? , ?, ? ,?, ? ,? ] (замінити ‘?’ відповідними
значеннями)
● Код програми, або опис/скан шляху розв’язку
