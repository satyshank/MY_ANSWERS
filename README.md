# MY_ANSWERS
INTERVIEW ANSWERS Coded Using JAVA

QUESTION 1: 

public class PYRAMID_RUNNER {

	public static void main(String[] args) {

		int i, j;
		int n = 4;
		for (i = 1; i <= n; i++) {

			for (j = 1; j <= n - i; j++) { // PRINTING SPACE
				System.out.printf(" ");
			}
			for (j = 1; j <= i; j++) { // PRINTING ASCENDING
				System.out.printf("%c", (char) (j + 64));
			}
			for (j = i - 1; j >= 1; j--) { // PRINTING DESCENDING
				System.out.printf("%c", (char) (j + 64));
			}

			System.out.println();
		}
	}

}

QUESTION2:

import java.util.Scanner;

public class duplicateRemover {

	public static void main(String[] args) {
		Scanner STRING = new Scanner(System.in);
		System.out.println("TYPE SOMETHING");
		String givenString = STRING.next();
		char[] GivenString = givenString.toCharArray();

		StringBuilder SB = new StringBuilder();
		for (int i = 0; i < GivenString.length; i++) {
			boolean ifrepeats = false;
			for (int j = i + 1; j < GivenString.length; j++) {
				if (GivenString[i] == GivenString[j]) {
					ifrepeats = true;
					break;

				}
			}
			if (!ifrepeats) {
				SB.append(GivenString[i]);
			}
		}

		System.out.println(SB);
	}

}
