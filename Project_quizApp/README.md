This is frontend Template for Quiz App using Html, CSS and JavaScript
public class FinalKeywordProgram {
    public static final int MAX_SIZE = 10; // Constant variable

    public static void main(String[] args) {
        final int localVar = 5; // Final local variable
        System.out.println("Local Variable: " + localVar);

        // Uncommenting the line below will result in a compilation error
        // localVar = 10; // Error: Cannot assign a value to final variable 'localVar'

        final StringBuilder finalStringBuilder = new StringBuilder("Hello");
        System.out.println("Original StringBuilder: " + finalStringBuilder);

        finalStringBuilder.append(" World"); // Modifying the object referred by final reference variable
        System.out.println("Modified StringBuilder: " + finalStringBuilder);

        final int[] finalArray = { 1, 2, 3 };
        System.out.println("Original Array: " + java.util.Arrays.toString(finalArray));

        finalArray[0] = 10; // Modifying elements of the final array
        System.out.println("Modified Array: " + java.util.Arrays.toString(finalArray));

        // Uncommenting the line below will result in a compilation error
        // finalArray = new int[] { 4, 5, 6 }; // Error: Cannot assign a value to final variable 'finalArray'
    }
}