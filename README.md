# Question-Five
Assignment
// This program is a simple calculator that can perform basic operations (+, -, * and /).

import java.util.Scanner;

public class Calculator {

    public static void main(String[] args) {

        // Create a Scanner object to read user input.
        Scanner scanner = new Scanner(System.in);

        // Ask the user to enter a number.
        System.out.println("Enter a number: ");
        double number1 = scanner.nextDouble();

        // Ask the user to enter an operation.
        System.out.println("Enter an operation (+, -, *, or /): ");
        String operation = scanner.next();

        // Ask the user to enter another number.
        System.out.println("Enter another number: ");
        double number2 = scanner.nextDouble();

        // Calculate the result of the operation.
        double result = 0.0;
        switch (operation) {
            case "+":
                result = number1 + number2;
                break;
            case "-":
                result = number1 - number2;
                break;
            case "*":
                result = number1 * number2;
                break;
            case "/":
                result = number1 / number2;
                break;
        }

        // Display the result.
        System.out.println(number1 + " " + operation + " " + number2 + " = " + result);
    }
}
