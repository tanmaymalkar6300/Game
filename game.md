import java.util.Random;
import java.util.Scanner;
	public class GuessTheNumber{


public static void main(String[] args) {
Random ran = new Random();
int randomNumber = ran.nextInt(100);
int attempts=0;

Scanner scanner = new Scanner(System.in);
System.out.println("Welcome to Guess the Number game.");
System.out.println("Try to Guess the Number between 1 to 100");

while(true) {
System.out.println("Enter the Guess Number");
int guess = scanner.nextInt();
 attempts++;
 
 if(guess<randomNumber) {
	 System.out.println("Too low! Try again");
	 
 }else if (guess> randomNumber) {
	 System.out.println("Too high! try again");
	 
 }
 else {
	 System.out.println("Congratulation u won the game");
	 break;
 }
	 
 }
scanner.close();
	
}
}
