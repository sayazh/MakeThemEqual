# MakeThemEqual
String exercise
package stringAssignments;

import java.util.Scanner;

public class MakeThemEqual {
	public static void main(String[] args) {

		Scanner scan = new Scanner(System.in);
		System.out.println("Enter your first word");
		String word1 = scan.next();
		System.out.println("Enter your second word");
		String word2 = scan.next();

		if (word1.length() == word2.length()) {
			System.out.println(word1);
			System.out.println(word2);
		} else if ( word1.length() > word2.length()) {
			System.out.println(word1.substring(0, word1.length() - 1) + "" + word2);
		} else if (word1.length() < word2.length()) {
			System.out.println(word1 + "" + word2.substring(0,word2.length() - 1));
		}
		scan.close();
	}
}
