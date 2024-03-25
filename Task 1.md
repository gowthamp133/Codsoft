# Codsoft
Number game
import java.util.*;
public class Main {
	public static void main(String[] args) {
		int n;
	    Scanner s=new Scanner(System.in);
	    Random r=new Random();
	    int random=r.nextInt(100);
	    System.out.println("Lets begin!");
 	   for(int i=1;i<=10;i++)
	    {
	          System.out.println("Guess the number : "); 
	          n=s.nextInt();
	          if(n<random){
	          System.out.println("The number is low"+"\nTry again!");
	        }
	        else if(n>random){
	        System.out.println("The number is high"+"\nTry again!");
	        }
	        else if(n==random){
	        System.out.println("You guessed correctly."+"\nYou win : )");
	        System.out.println("Your score : "+10*(11-i)+"/100");
	        break;
	        }
	    }
	   System.out.println("The random number is : "+random);	    
	}
}
