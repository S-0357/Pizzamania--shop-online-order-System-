# Pizzamania Ordering System

## Overview
The **Pizzamania Ordering System** is a Java-based console application designed to simulate the process of ordering pizzas. The application provides options for different types of pizzas, customizations, and billing. It demonstrates key object-oriented programming principles, including inheritance and encapsulation.

## Features
- **Pizza Categories:**
  - Veg Pizza
  - Non-Veg Pizza
  - Deluxe Veg Pizza
  - Deluxe Non-Veg Pizza
- **Customization Options:**
  - Add extra cheese.
  - Add extra toppings.
  - Opt for takeaway.
- **Billing System:** Automatically calculates the total cost based on user choices and displays a detailed bill.
- **Code Structure:** Leverages OOP concepts such as inheritance, method overriding, and encapsulation for code modularity.

## Code Structure
### Main Components
1. **`pizza` Class:**
   - Represents a base pizza with options for customization.
   - Attributes:
     - `price` - Total cost of the pizza.
     - `veg` - Boolean indicating if the pizza is vegetarian.
     - `extraCheesePrice`, `extraToppingsPrice`, `backPackPrice` - Costs for additional options.
   - Methods:
     - `addExtraCheese()` - Adds cheese to the pizza and updates the price.
     - `addExtraToppings()` - Adds toppings to the pizza and updates the price.
     - `takeAway()` - Adds takeaway option and updates the price.
     - `getBill()` - Displays a detailed bill.
   
2. **`DeluxPizza` Class:**
   - Inherits from the `pizza` class.
   - Overrides methods to automatically add extra cheese and toppings without user input.
   - Designed specifically for deluxe pizza options.

3. **`Main` Class:**
   - Entry point for the application.
   - Handles user input to select pizza type and apply customizations.
   - Uses a `switch` statement to instantiate and process different pizza types.

## How to Run the Application
### Prerequisites
1. Java Development Kit (JDK) installed.
2. A code editor or IDE (e.g., Eclipse, IntelliJ IDEA, or VS Code).

### Steps to Execute
1. Clone or download the project files.
2. Open the project in your preferred IDE or compile the `.java` files manually.
3. Run the `Main` class to start the application.
4. Follow the prompts to:
   - Select a pizza type.
   - Choose customization options.
   - View the final bill.

### Example Interaction
1. Application starts with a welcome message and pizza options.
2. User selects "Veg Pizza" and adds extra cheese and toppings.
3. User opts for takeaway.
4. Application displays a detailed bill:
   ```
   --------------------Welcome to Pizzamania---------------------
   Pizza : 300
   Extra Cheese : 100
   Extra Toppings : 150
   Take away : 20
   
   Total Amount: 570

   Thank you!!! Visit Again.....
   --------------------------------------------------
   ```

## Key OOP Concepts Demonstrated
- **Inheritance:** The `DeluxPizza` class extends the `pizza` class to inherit its properties and methods.
- **Method Overriding:** Deluxe pizzas automatically include extras by overriding the `addExtraCheese` and `addExtraToppings` methods.
- **Encapsulation:** Sensitive attributes like `price` and customization flags are kept private/protected.

## Future Enhancements
- Add GUI support for a more interactive experience.
- Integrate a database for managing orders and tracking sales.
- Implement multiple payment methods.



