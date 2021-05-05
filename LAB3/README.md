# Звіт із лабораторної роботи №3
---
### із дисципліни Теоретичні основи телекомунікацій
## Тема: *Методи обходу та модифікації графів.*
---
## Мета роботи: *Навчитись застосовувати алгоритми обходу графів, побудови дерева шляхів та мінімального зв’язного дерева.*

### Виконав: студент групи *ТР-32* Заяць Н.А.
### Прийняв: викладач Бугиль Б.А.
---

### Виконання роботи
#### 1.	За допомогою лабораторного макету побудувати випадковий неорієнтований граф G={8,12}:
![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/1.png)

i.	Побудувати дерево за алгоритмом обходу в ширину (BFS); (для 2-х різних вершин)
* Для вершини 6 порядок обходу: 6 1 5 8 2 4 7 3

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/2.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/3.png)

* Для вершини 8 порядок обходу: 8 1 3 6 2 4 7 5

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/4.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/5.png)

ii.	Чи будуть однаковими топології дерев побудованих з різних кореневих вершин? Чому?
* Так, тому що на виході із вершини 6 і 8 корінь в обох має по три вершини.


iii.	Побудувати дерево за алгоритмом обходу в глибину (DFS); (для 2-х різних вершин)
* Для вершини 1 порядок обходу: 1 2 4 3 7 5 6 8

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/6.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/7.png)


* Для вершини 3 порядок обходу: 3 4 2 1 6 5 7 8

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/8.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/9.png)

iv.	Чи будуть однаковими топології дерев побудованих з різних кореневих вершин? Чому?
* Ні, тому що у другому графі вершина 6 у своєму подальшому послідовному корені вершин 5-7 потрапила у глухий кут і їй довелось вернутись, так як ще одна вершина не була знайдена.

#### 2.	За допомогою лабораторного макету побудувати випадковий орієнтований граф G={6,10}:

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/10.png)

i.	Побудувати дерево за алгоритмом обходу в ширину (BFS);
* Порядок обходу: 1 2 3 5 6 4

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/11.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/12.png)

ii.	Яка вершина (вершини) буде знайдена останньою?
* Вершина 4

iii.	Визначити чи існують цикли. Вказати послідовність ребер і їх довжину.
* Цикли: 1-2-6-1 (довжина 3), 1-3-4-6-1 (довжина 4), 2-6-4-2 (довжина 5), 

iv.	Визначити кількість хвиль, які пройдуть по ребрах доки буде виявлена остання вершина.
* Кількість хвиль становить 5.

v.	Побудувати дерево за алгоритмом обходу в глибину (DFS);
* Порядок обходу: 1 2 5 3 4 6

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/13.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/14.png)

#### 3.	Побудувати дерево шляхів рангом r=4 для випадкового графа G={6,9}.

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/15.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/16.png)

#### 4.	Побудувати мінімальне зв’язне дерево для графа G. Вказати його вагу.

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/17.png)

![image](https://github.com/ZaiatsNazarii/nazariizaiats/blob/main/LAB3/18.png)


* Вага: 5+7+9+3+5=29
