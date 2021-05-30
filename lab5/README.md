# Звіт до лабораторної роботи №5

### Тема: Визначення максимального потоку

### Мета роботи: Навчитись знаходити максимальний потік між парою вузлів та визначати мінімальний переріз.

## Виконання роботи:
![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/lab5/3.jpg)


#### 1) Для заданого графа G {8,10}, знайти шлях (вказати послідовність ребер) з максимальною пропускною здатністю (вказати якою) між вузлами 1 та 5. 
Від вершини 1 до вершини 5 згідно алгоритму Флойда шлях з максимальною пропускною здатність і одночасно найкоротший це через вершини  1->2->4->5=1. Його пропускна здатність становитиме 1, як і ребро з мінімальним ваговим коефіцієнтом в цьому шляху

#### 2)  Визначити максимальний потік, який може бути переданий між вузлами 1 та 5
Максимальний потік, який може бути переданий між вузлами 1 та 5 становить:
1->2->4->5=13
1->8->3->4->5=21
1->2->7->6->5=16
1->8->6->5=19
Максимальний потік - 69

#### 3)  Вказати ребра, які входять у мінімальний переріз.
У мінімальний переріз входять ребра 1-2, 2-4, 4-5. 

#### 4) Визначити максимальний потік, який може виходити з вузла 1. Визначити максимальний потік, який може входити у вузол 1. 
Максимальний потік, який може виходити з вузла 1 становить: 1-2=1, 1-8=6 максимальний потік – 7.
Максимальний потік, який може входити у вузол 5 становить: 6->5=5, 4->5=2 
максимальний потік – 7.
Вважаючи, що між вузлами 1 та 5 передається максимальний потік, до яких вузлів можна здійснити передачу інформації з вузла 1. Визначити пропускну здатність даних маршрутів.
1-2=1 пропускна здатність 1
1-8=6 пропускна здатність 6
1-8-3=10 пропускна здатність 4
1-8-3-4=19 пропускна здатність 4
1-8-3-4-5=21  пропускна здатність 2
1-8=6 пропускна здатність 6
1-8-5=11 пропускна здатність 5
1-2-7=8 пропускна здатність 1
1-2-7-6=11 пропускна здатність 1
1-2-7-6-5=16 пропускна здатність 1

#### 5) Вважаючи, що між вузлами 1 та 5 передається максимальний потік, які вузли можуть здійснити передачу інформації до вузла 5. Визначити пропускну здатність даних маршрутів.
4-5=2 пропускна здатність 2
3-4-5=11 пропускна здатність 2
8-3-4-5=15 пропускна здатність 2
1-8-3-4-5=21 пропускна здатність 2
2-4-5= 12 пропускна здатність 2
1-2-4-5= 13 пропускна здатність 1
6-5=5 пропускна здатність 5
7-6-5=8 пропускна здатність 3
2-7-6-5=15 пропускна здатність 3
1-2-7-6-5=16 пропускна здатність 1

Висновок: було визначено максимальний потік між 1 і 5 вершинами, і становить - 69 використовуючи алгоритм Флойда.