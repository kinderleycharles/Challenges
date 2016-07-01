import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        Scanner scan = new Scanner(System.in);
        int testCases = scan.nextInt();
        scan.nextLine();                        // Eat \n character
        
        // Initialize array contents to 0
        int[] alphabet = new int[26];
        int gemCounter = 100;
        for(int i = 0; i != 26; ++i) {
            alphabet[i] = 0; 
        }
        
        String str = "";
        for(int i = 0; i != testCases; ++i) {
            str = scan.nextLine();
            int lineGem = 0;
            if(i == 0) { lineGem = str.length(); }
            for(int j = 0; j != str.length(); ++j) {
                int aID = (int)((int)str.charAt(j)-97);
                // Initialize array for very first loop
                if((i != 0) && (alphabet[aID] == i)){
                    lineGem++;
                }
                alphabet[aID] = i+1;
            }
                   
            if ((i != 0) && (lineGem <= gemCounter)) { 
                gemCounter = lineGem; 
            }
        }
        
        System.out.println(gemCounter);
    }
}
