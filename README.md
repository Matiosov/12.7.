# 12.7.3
МОДУЛЬ 12, ЗАДАЧА 12.7.3

Задание 12.7.3 Вам дан словарь per_cent с распределением процентных ставок по вкладам в различных банках таким образом, что ключ — название банка, значение — процент. 
	Напишите программу, в результате которой будет сформирован список deposit значений — накопленные средства за год вклада в каждом из банков. На вход программы с клавиатуры вводится сумма money, которую человек планирует положить под проценты. per_cent = {'ТКБ': 5.6, 'СКБ': 5.9, 'ВТБ': 4.28, 'СБЕР': 4.0} = {} Пример работы программы при money = 100000 deposit = [5600, 5900, 4280, 4000] Для самостоятельного изучения вам была дана ссылка на методы для работы со списками. Изучите методы и найдите тот, который позволяет найти максимальное значение среди элементов в списке. 
	Добавьте в программу поиск максимального значения и его вывод на экран в формате: Максимальная сумма, которую вы можете заработать — deposit[i] Где вместо deposit[i] будет выведено максимальное значение списка.

Решение. per_cent = {'ТКБ': 5.6, 'СКБ': 5.9, 'ВТБ': 4.28, 'СБЕР': 4.0} money = int(input('Введите сумму вклада')) deposit = [] for key in per_cent: deposit.append(per_cent[key] * money / 100) max_deposit = max(deposit) print(deposit) print ("Максимальная сумма, которую вы можете заработать — " + str(max_deposit))

C:\PYTON\PROJECTS\MDS\12.7\venv\Scripts\python.exe C:\PYTON\PROJECTS\MDS\12.7\main.py 
Введите сумму вклада100000
[5600.0, 5900.0, 4280.0, 4000.0]
Максимальная сумма, которую вы можете заработать — 5900.0

Process finished with exit code 0
