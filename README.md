# Geley Tsebe Gurung
## JAVA is a programming language and computing platform that's used to create many applications,
![JAVA](https://github.com/Zzingeley/new-era/blob/main/images/How-java-code-executes.png)

// Define a class
class Animal {
    // Attributes
    String name;
    int age;

    // Constructor
    public Animal(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Method
    public void makeSound() {
        System.out.println(name + " makes a sound!");
    }
}

// A subclass that inherits from Animal
class Dog extends Animal {
    // Constructor
    public Dog(String name, int age) {
        super(name, age); // Call the parent class constructor
    }

    // Overridden method
    @Override
    public void makeSound() {
        System.out.println(name + " says: Woof woof!");
    }
}

// Main class to run the program
public class Main {
    public static void main(String[] args) {
        // Create an instance of Animal
        Animal genericAnimal = new Animal("Generic Animal", 3);
        genericAnimal.makeSound();

        // Create an instance of Dog (subclass of Animal)
        Dog dog = new Dog("Buddy", 5);
        dog.makeSound();

        // Display information
        System.out.println("Name: " + dog.name);
        System.out.println("Age: " + dog.age);
    }
}

