
import java.util.Scanner;
import java.lang.Math;

public class coinChange {
	public static void main(String[] args) {
   
   
	   //Display welcome message
	   System.out.println("Welcome to the magical change calculator!");

	   
	  // get user input of change
	  Scanner myScanner = new Scanner(System.in);
	  System.out.print("\nEnter the total amount of change: ");
	  int totalAmt = myScanner.nextInt();
      
      // define variables for coins
      int quarter = 25;
      int dime = 10;
      int nickel = 5;
      int penny = 1;
      
      // count number of coins
      int numQuarters = (int)(totalAmt / quarter);
      	totalAmt %= quarter;
      	
      int numDimes = (int)(totalAmt / dime);
      	totalAmt %= dime;
      
      int numNickels = (int)(totalAmt / nickel);
      	totalAmt %= nickel;
      
      int numPennies = (int)(totalAmt / penny);
      	totalAmt %= penny;
      
      // return information to user
      System.out.println("Number of quarters to give: " + numQuarters + "\n" + 
    		  "Number of dimes to give: " + numDimes + "\n" +
    		  "Number of nickels to give: " + numNickels + "\n" +
    		  "Number of pennies to give: " + numPennies);
       }
}
