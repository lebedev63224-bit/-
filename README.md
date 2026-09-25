def calculator():
    # Ввод чисел
    number1 = float(input("Введите первое число: "))
    number2 = float(input("Введите второе число: "))
    
    # Ввод операции
    operation = input("Выберите операцию (+, -, *, /): ")
    
    # Вычисления
    if operation == '+':
        result = number1 + number2
    elif operation == '-':
        result = number1 - number2
    elif operation == '*':
        result = number1 * number2
    elif operation == '/':
        if number2 == 0:
            result = "Ошибка: деление на ноль!"
        else:
            result = number1 / number2
    else:
        result = "Неверная операция!"
    
    # Вывод результата
    print("Результат:", result)

# Запуск калькулятора
calculator()
