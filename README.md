# cats
class Cat:
    def __init__(self, name, breed, age):
        self.name = name
        self.breed = breed
        self.age = age
        self.is_sleeping = False

    def meow(self):
        return "Meow!"

    def sleep(self):
        self.is_sleeping = True
        return f"{self.name} is now sleeping."

    def wake_up(self):
        self.is_sleeping = False
        return f"{self.name} woke up!"

def main():
    # Creating a cat object
    my_cat = Cat("Whiskers", "Persian", 5)

    # Accessing attributes
    print(f"My cat's name is {my_cat.name}.")
    print(f"My cat's breed is {my_cat.breed}.")
    print(f"My cat is {my_cat.age} years old.")

    # Calling methods
    print(my_cat.meow())
    print(my_cat.sleep())
    print(my_cat.wake_up())

if __name__ == "__main__":
    main()
