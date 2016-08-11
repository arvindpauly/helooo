# helooo

import java.util.Scanner;

public class Guvi2 {
	public static void main(String[] args) {
		Scanner a = new Scanner(System.in);
		System.out.println("enter the string");
		String s1 = a.next();
		StringBuffer s = new StringBuffer("");
		for (int i = 0; i < s1.length(); i++) {
			if (i != s1.length() - 1) {
				if (s1.charAt(i) == s1.charAt(i + 1)) {
					s.append(s1.charAt(i));
					s.append('*');
					continue;

				} else {
					s.append(s1.charAt(i));
				}
			} else {
				s.append(s1.charAt(i));
			}

		}
		System.out.println(s);
		a.close();
	}
}
