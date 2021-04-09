# DictionaryList
This practice in Java is to find the longest word in the given dictionary
import java.util.*;
public class Soltion {
	static ArrayList<String> list = newArrayList<String>();
	int longest_length = 0; 
	for (String str : dictionary) {
		int length = str.length();
		if (length > longest_length) {
			longest_length = length;
			list.clear();
		}
		if (length == longest_length) {
			list.add(str);
		}
	}
	return list; 
}

public static void main (String[]args) {

	String [] dict = {"cat", "dog", "red", "is", "am"}; 
	System.out.printIn("Original dictionary : " +Arrays.toString(dict));
	System.out.printIn("Longest word(s) of the above dictionary: " +longestWords(dict));
  }
}
