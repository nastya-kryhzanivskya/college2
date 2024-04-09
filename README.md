### Знайомство з ООП

## Створюємо перший class

1 - <img width="1440" alt="Знімок екрана 2024-04-09 о 12 07 31" src="https://github.com/nastya-kryhzanivskya/college2/assets/154334074/fe17bf62-b7b7-431f-8392-792c417ff23d">

5 - 

1. При передачі значення None створюється об'єкт з іменем "Anonymous", оскільки відсутнє ім'я не може бути відображено. Це ім'я використовується як ім'я за замовчуванням, коли ім'я не передається явно.

2. Щоб змінити текст привітання при виклику методу say_hello(), можна змінити текст у методі самого класу. Ось як це можна зробити:
   
class Greeting:
    def say_hello(self):
        print("Привіт, світе!")
    def custom_greeting(self, text):
        print(text)

greet = Greeting()
greet.say_hello()  # Виведе: Привіт, світе!
greet.custom_greeting("Це нове привітання!")  # Виведе: Це нове привітання!

3. Доповнена функція в класі, яка порахує кількість букв у імені:
class Greeting:
    def __init__(self, name):
        self.name = name

    def say_hello(self):
        print("Привіт,", self.name)

    Функція для підрахунку кількості букв у імені
    def count_letters(self):
        return len(self.name)

greet = Greeting("Василь")
greet.say_hello()  # Виведе: Привіт, Василь
print("Кількість букв у імені:", greet.count_letters())  # Виведе: Кількість букв у імені: 6

4. Різниця у кількості імен у списку names та підрахунку може бути через різницю у використанні пробілів або інших символів, які можуть бути враховані в різних реалізаціях. Для точної порівняння потрібно впевнитися, що список ім'я і підрахунок виконані на одних і тих же даних і за однаковими правилами.
