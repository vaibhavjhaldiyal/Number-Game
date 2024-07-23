import java.util.Random;
import java.util.Scanner;
import java.util.random.*;
public class Number_Game {
public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    System.out.println("WELCOME TO THE NUMBER GAME");
    Random rn = new Random();
    int number = rn.nextInt(100);
    System.out.println("Enter the number between 1 to 100");
    while (number<100) {
    int user_number = sc.nextInt();
    if(number == user_number){
        System.out.println("CONGRATULATIONS! YOU GUESSED THE CORRECT NUMBER <3");
        break;
    }
    else if(number > user_number){
        System.out.println("ENTER A GREATER NUMBER:");
    }
    else if(number < user_number){
        System.out.println("ENTER A LESSER NUMBER:");
    }
    else{
        System.out.println("INVALID NUMBER");
    }
}
}
    
}
