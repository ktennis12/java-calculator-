# java-calculator-
A calculator in java program

import java.util.Scanner; // Import the Scanner class

class Calculator {
    private static void calculation(Integer num1, Integer num2, char op) {
        if (op == '+') {
            Integer answer_add = num1 + num2;
            System.out.println(answer_add);
        } else if (op == '-') {
            Integer answer_sub = num1 - num2;
            System.out.println(answer_sub);
        } else if (op == '*') {
            Integer answer_multi = num1 * num2;
            System.out.println(answer_multi);
        } else if (op == '/') {
            Integer answer_div = num1 / num2;
            System.out.println(answer_div);
        }
    }

    public static void main(String[] args) {
        Scanner myObj = new Scanner(System.in); // Create a Scanner object

        System.out.println("Give a number to the calculator.");
        Integer number1 = myObj.nextInt(); // Read user input
        System.out.println("Give another number to the calculator. ");
        Integer number2 = myObj.nextInt();
        System.out.println("Give the calculator an operator. ");
        char operation = myObj.next().charAt(0);

        calculation(number1, number2, operation);
    }
}
