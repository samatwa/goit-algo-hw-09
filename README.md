# goit-algo-hw-09
 
# Порівняння ефективністі жадібного алгоритму та алгоритму динамічного програмування, базуючись на часі їх виконання, за допомогою timeit
Виконання цього коду дасть нам чітке уявлення про те, який з алгоритмів швидше для конкретної суми (в даному випадку 113).

Результати виконання (при $number=100000$):
 - Час виконання жадібного алгоритму: $0.083812$ секунд
 - Час виконання алгоритму динамічного програмування: $6.854841$ секунд\
(Результати можуть варіюватися в залежності від обчислювальної потужності системи, на якій виконується код)

Висновки:
 - Жадібний алгоритм: Виконується набагато швидше, оскільки він здійснює лише один прохід по номіналах монет. Це робить його ідеальним для використання в реальних застосуваннях, де час відповіді має бути мінімальним.
 - Алгоритм динамічного програмування: Хоча і забезпечує оптимальне рішення, але має значно більшу обчислювальну складність і, відповідно, більший час виконання. Це робить його менш практичним для використання в ситуаціях, де потрібна швидкість.
 - Жадібний алгоритм підходить для більшості реальних застосувань, де набір монет дозволяє знаходити оптимальне рішення швидко. Алгоритм динамічного програмування варто використовувати лише тоді, коли важлива гарантована оптимальність і немає жорстких вимог до часу виконання.

# Порівняння ефективністі жадібного алгоритму та алгоритму динамічного програмування, базуючись на О великому
Жадібний алгоритм
Час виконання: O(n), де n – кількість номіналів монет.
Продуктивність: Швидко видає рішення, однак не завжди оптимальне для всіх наборів монет.
Справляється з великими сумами: Добре підходить для великих сум при умові, що набір монет дозволяє оптимальні розрахунки.
Жадібний алгоритм є дуже ефективним з точки зору часу виконання. Він підходить для практичного використання в більшості випадків, особливо коли номінали монет складаються таким чином, що жадібний підхід завжди дає оптимальний результат (наприклад, як у випадку з українськими гривнями). Однак, якщо набір монет був би іншим (наприклад, [9, 6, 5, 1]), жадібний алгоритм міг би не знайти оптимальне рішення.

Алгоритм динамічного програмування
Час виконання: O(amount * n), де amount – сума, яку потрібно видати, n – кількість номіналів монет.
Продуктивність: Завжди знаходить оптимальне рішення, мінімізуючи кількість монет.
Справляється з великими сумами: Може бути повільним для дуже великих сум через високу обчислювальну складність, але завжди дає мінімальну кількість монет.
Алгоритм динамічного програмування гарантує, що ми отримаємо найменшу кількість монет для видачі решти. Однак, це приходить з більш високою обчислювальною вартістю. Якщо сума є дуже великою, алгоритм може бути повільним, але він завжди надає оптимальний результат.

Висновки:
Жадібний алгоритм є більш ефективним у плані часу виконання і підходить для більшості практичних випадків, де набір монет дозволяє оптимальні розрахунки. Алгоритм динамічного програмування, хоча і має вищу обчислювальну складність, гарантує мінімальну кількість монет, що може бути критичним для певних наборів монет.

Вибір алгоритму залежить від конкретних вимог до оптимальності та швидкості виконання. Якщо швидкість є критичною, а набір монет є сприятливим для жадібного підходу, жадібний алгоритм буде кращим вибором. Якщо ж потрібна гарантована оптимальність незалежно від набору монет, варто використовувати алгоритм динамічного програмування.