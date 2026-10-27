This program is a Cafe Ordering System that displays food and drink orders, calculates the subtotal and discounts, and determines the total payment.

Structure of the Files
- MenuItem.java — an abstract parent class for all menu items.
- Discountable.java — an interface that defines the behavior for calculating discounts.
- Food.java — a subclass of MenuItem representing food items.
- Drink.java — a subclass of MenuItem representing drink items.
- Order.java — manages menu items and calculates the subtotal, total discounts, and final payment.
- Main.java — the main class that demonstrates how the program works.

OOP Concepts Implemented
1. Abstract Class
MenuItem is an abstract class because it serves as a base class for different types of menu items rather than representing a specific menu item. It contains common attributes, such as name and price.

2. Abstract Method
calculatePrice() is declared as an abstract method in MenuItem without a method body. The Food and Drink subclasses must provide their own implementations of this method.

3. Interface
Discountable defines the calculateDiscount() method. Both Food and Drink implement this interface, but they can have different discount calculation rules.

4. Inheritance
Food extends MenuItem and Drink extends MenuItem. Both subclasses inherit attributes and methods from the MenuItem parent class.

5. Polymorphism
In Main, variables of type MenuItem are used to store Food and Drink objects. When Order calls the displayDetails() or calculatePrice() methods, the implementation that executes depends on the actual type of the object. This demonstrates polymorphism in Java.