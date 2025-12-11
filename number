print("Гра: комп'ютер вгадує ваше число методом бісекції!")

# Введення верхньої межі n
n = int(input("Введіть максимальне число n: "))

low = 1
high = n
steps = 0

print(f"Загадайте число від 1 до {n}. Я починаю вгадувати!")

while True:
    steps += 1
    guess = (low + high) // 2
    print(f"\nМоя спроба №{steps}: Число {guess}?")

    answer = input("Це ваше число? (так/ні): ").strip().lower()

    if answer == "так":
        print(f"\nЯ вгадав ваше число {guess} за {steps} ходів!")
        break
    
    # Якщо не вгадав — уточнюємо напрямок
    direction = input("Ваше число більше чи менше? (більше/менше): ").strip().lower()

    if direction == "більше":
        low = guess + 1
    elif direction == "менше":
        high = guess - 1
    else:
        print("Невідома відповідь, повторіть ще раз.")
        steps -= 1  # не рахуємо некоректний крок
