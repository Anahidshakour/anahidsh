package practise;
import java.util.Scanner;

public class prac {
	public static void main(String args[]) {
		
		Scanner input = new Scanner(System.in);
		System.out.println("please enter your name");
		Test2 object = new Test2();
		String usernames = input.nextLine();

		object.method1(usernames);
		object.method2();
		object.agemethod();
		object.calculater();
		
		System.out.println("Do you want more calculation?");
		Scanner yn = new Scanner(System.in);
		String yno = yn.nextLine();
		
		while(yno.equals("yes") || yno.equals("no")) {
			
			if(yno.equals("yes")) {
				object.calculater();
			}
			
			if (yno.equals("no")) {
				
				System.out.println("thanks, goodbye " + usernames);
				break;
				
			}else {
				
				System.out.println("please answer with yes or no");
			}
			
			System.out.println("any more calculation?");
			String yno1 = yn.nextLine();
			yno = yno1;
		}
	}

}

