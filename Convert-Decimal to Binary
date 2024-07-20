import java.util.Scanner;
import java.util.Stack;

public class DecimalToBinary {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a positive decimal number: ");
        int decimalNumber = scanner.nextInt();

        // Check if the number is negative
        if (decimalNumber < 0) {
            System.out.println("Please enter a positive decimal number.");
            return;
        }
      
        // Convert to binary and display the result
        String binaryString = decimalToBinary(decimalNumber);
        System.out.println("Binary equivalent: " + binaryString);
    }

    // Method to convert decimal to binary
    public static String decimalToBinary(int number) {
        if (number == 0) {
            return "0";
        }

        Stack<Integer> remainders = new Stack<>();

        // Perform the conversion by dividing the number by 2
        while (number > 0) {
            int remainder = number % 2;
            remainders.push(remainder);
            number = number / 2;
        }

        // Construct the binary string from the stack
        StringBuilder binaryString = new StringBuilder();
        while (!remainders.isEmpty()) {
            binaryString.append(remainders.pop());
        }

        return binaryString.toString();
    }
}
