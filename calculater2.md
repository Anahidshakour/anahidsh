package practise;
import java.util.Scanner;
public class Test2 {
	private String username;

	public void method1(String userName) {
		username = userName;
	}

	public void method2() {
		System.out.println("Hello " + username + " nice to meet you");
	}

	public void agemethod() {

		System.out.println("please enter your age ");
		Scanner ageinput = new Scanner(System.in);
		String ages = ageinput.nextLine();
		System.out.println(username + " you are " + ages + " years old.");

	}

	public void calculater() {

		System.out.println("please type in your first number");
		Scanner numinput = new Scanner(System.in);
		int number1 = numinput.nextInt();

		System.out.println("please type in your second number");
		Scanner numinput2 = new Scanner(System.in);
		int number2 = numinput.nextInt();

		System.out.println("please typle in the maths symbol needed between the numbers");
		Scanner symbolin = new Scanner(System.in);
		String symbol = symbolin.nextLine();
		double answer;
		switch (symbol) {
		case "+" :
			System.out.println(answer = number1 + number2); 
			break;
		case "-" :
			System.out.println(answer = number1 - number2);
			break;
		case "*" :
			System.out.println(answer = number1 * number2);
			break;
		case "/" :
			System.out.println(answer = number1 / number2);
			break;
		default:
			System.out.println("wrong symbol");
			break;
		}
	}
}

