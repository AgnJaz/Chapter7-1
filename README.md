import java.util.Scanner;

public class Array {
	public static void main(String[] args) {
		int[] array = new int[8];

		System.out.print("Enter eight integers: ");

		fill(array);

		for (int i = array.length - 1; i >= 0; i--)
			System.out.print(array[i] + " ");
		System.out.println();
	}

	public static void fill(int[] array) {
		Scanner input = new Scanner(System.in);
		for (int i = 0; i < array.length; i++) 
			array[i] = input.nextInt();
	}
}
