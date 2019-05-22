# GuessName
Steam Fest
import java.util.Scanner;

public class Nams_Age {

	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		System.out.println("Hello! My name is Vikki");
		System.out.println();
		System.out.println("What is your name? Please Type it");
		String name = input.nextLine();
		System.out.println("Hello " + name + " You have a really nice name");
// System.out.println("How old are you? I am 5 years old! ");
// int age = input.nextInt();
// System.out.println();
// System.out.println("Wow! " + age + " years old.... you are old");

		System.out.println("Do you want to play a game with me? Enter true to Play or false to not Play");

		boolean answer = input.nextBoolean();

		if (answer == true) {
			System.out.println("Yay let play!");
			System.out.println("I will guess how old you are");
			System.out.println("First Pick any number between 1 -10");
			int guess = input.nextInt();

			int temp = (guess * 2);
			//System.out.println(temp);
			int temp2 = (temp + 5);
			//System.out.println(temp2);
			int temp3 = (temp2 * 50);
			//System.out.println(temp3);


			System.out.println("Ok has your bday already passed this year? Enter true for yes enter false for no");
			boolean response = input.nextBoolean();
			if (response == true) {
				System.out.println("Happy belated Bday. hmm I am still thinking");
				int temp4 = (temp3 + 1767);
				System.out.println("What Year were you born?");
				int year = input.nextInt();
				int temp5 = temp4-year;
				//System.out.println(temp5);

				System.out.println("Ok I think I know !");
				System.out.println(temp5);
				System.out.println("The frirst number is your guess and the last two numbers are your age ");
				System.out.println("Did I guess right!!");
				
			} else {
				System.out.println(" hmm I am still thinking");
				System.out.println("What Year were you born?");
				int year = input.nextInt();
				int temp4 = (temp3 + 1768);
				//System.out.println(temp4);
				int temp5 = (temp4-year);
				
				System.out.println(temp5);
				System.out.println("The frirst number is your guess and the last two numbers are your age ");
				System.out.println("Did I guess right!!");

			}
		} else {
			System.out.println("Ok it was nice to meet you " + name + " bye bye");
		}
	}
}
