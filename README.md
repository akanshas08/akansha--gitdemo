# akansha--gitdemo

//ASSIGNMENT DAY 4
//QUES1
public class Main {
    public static void main(String[] args) {
        // Replace "yourInput" with the actual input you want to test
        String city = "Mumbai";

        switch (city) {
            case "Mumbai":
                System.out.println("Financial city");
                break;
            case "Kolkata":
                System.out.println("City of Joy");
                break;
            case "Delhi":
                System.out.println("Capital of the country");
                break;
            case "Bangalore":
                System.out.println("Cyber City");
                break;
            default:
                System.out.println("May be Other Indian City");
        }
    }
}


//ques2
public class CheckWeather {
    public static void main(String[] args) {
        // Assume these can have any value
        boolean isSnowing = false;
        boolean isRaining = true;
        double temperature = 60.0;

        // Check weather conditions
        if (isRaining || isSnowing || temperature < 50.0) {
            System.out.println("Let's stay home.");
        } else {
            System.out.println("Let's go out!");
        }
    }
}

//ques3
import java.util.Scanner;

public class CheckCharType {
    
    public void checkChar(char inputChar) {
        if ((inputChar >= 'a' && inputChar <= 'z') || (inputChar >= 'A' && inputChar <= 'Z')) {
            // Check if the character is a vowel
            if ("aeiouAEIOU".indexOf(inputChar) != -1) {
                System.out.println(inputChar + " is a vowel.");
            } else {
                System.out.println(inputChar + " is a consonant.");
            }
        } else {
            System.out.println("Error: Invalid character. Please enter a valid alphabet character.");
        }
    }

    public static void main(String[] args) {
        // Create an instance of the class
        CheckCharType charChecker = new CheckCharType();
        
        // Call the method with a vowel
        charChecker.checkChar('a');
        
        // Call the method with a consonant
        charChecker.checkChar('b');
        
        // Call the method with an invalid character
        charChecker.checkChar('1');
    }
}