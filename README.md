# CMSC203_Lab3
import java.util.Scanner;

public class MovieDriver {

		public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner input=new Scanner(System.in);
		char ch='y';
		while(ch=='y')
		{
		Movie m=new Movie();
		System.out.println("Enter the name of the movie : ");
		String title=input.nextLine();
		m.setTitle(title);//setting title
		System.out.println("Enter the rating of the movie : ");
		String rating=input.next();
		m.setRating(rating);//setting rating
		System.out.println("Enter the number of tickets sold for this movie : ");
		int n=input.nextInt();
		m.setSoldTickets(n);//setting no of tickets
		System.out.println(m.toString());
		System.out.println("Do you want to enter another ?(y or n)");
		ch=input.next().charAt(0);
		input.nextLine();//for line feed

		}

		System.out.println("Goodbye!");

		}
}
