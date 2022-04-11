import java.util.ArrayList;
import java.util.Arrays;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String enteredString = scanner.nextLine();

        oddAndEvenCheck(enteredString);

        digitCounter(enteredString);

        justNumbersString(enteredString);

        cleaneDublicates(enteredString);

        sybolCounter(enteredString);

        stringReverse(enteredString);

        subStrCount(enteredString);

        reverseSubStrs(enteredString);

        sortArray(enteredString);

        shortestWordLength(enteredString);

        wordsCount(enteredString);

        addSpace(enteredString);

        isItPolidrom(enteredString);

        changeSubStr(enteredString);

        subStrDistance(enteredString);
    }

    public static void oddAndEvenCheck(String s){
        char[] enteredRow = s.toCharArray();
        String oddRow = "";
        String evenRow = "";
        for (char symbol: enteredRow) {
            if(Character.isDigit(symbol)){
                if(symbol % 2 == 0){
                    evenRow += symbol;
                }
                else {
                    oddRow += symbol;
                }
            }
        }
        System.out.println(oddRow);
        System.out.println(evenRow);
    }

    public static void digitCounter(String s){
        int digits = 0;
        char[] enteredRow = s.toCharArray();
        for (char symbol: enteredRow) {
            if(Character.isDigit(symbol)){
                digits++;
            }
        }
        System.out.println(digits);
    }

    public static String justNumbersString(String s){
        String numbers = "";
        char[] enteredRow = s.toCharArray();
        for (char symbol: enteredRow) {
            if(Character.isDigit(symbol)){
                numbers += symbol;
            }
        }
        System.out.println(numbers);
        return numbers;
    }

    public static String cleaneDublicates(String s){
        String noDublicates = "";
        boolean charWas = false;
        for (char symbol: s.toCharArray()) {
            for (char dublicate: noDublicates.toCharArray()) {
                if(symbol == dublicate){
                    charWas = true;
                }
            }
            if(charWas != true){
                noDublicates += symbol;
            }
            charWas = false;
        }
        System.out.println(noDublicates);
        return noDublicates;
    }

    public static void sybolCounter(String s){
        Scanner charScanner = new Scanner(System.in);
        int charCount = 0;
        char enteredChar;
        System.out.println("Enter a symbol what you want to count");
        enteredChar = charScanner.next().charAt(0);
        for (char symbol: s.toCharArray()) {
            if(symbol == enteredChar){
                charCount++;
            }
        }
        System.out.println("Count of entered symbol in string: " + charCount);
    }

    public static String stringReverse(String s){
        String reversedString = "";
        for(int i = s.length() - 1; i >= 0; i--){
            reversedString += s.toCharArray()[i];
        }
        System.out.println(reversedString);
        return reversedString;
    }

    public static void subStrCount(String s){
        Scanner scanner = new Scanner(System.in);
        String subStr = scanner.next();
        System.out.println((s.length() - s.replace(subStr, "").length()) / subStr.length());
    }

    public static String reverseSubStrs(String s){
        String[] words = s.split("\\s");
        String reversed = "";
        String temp = "";
        for(int i = 0; i < words.length/2; i++){
         temp = words[i];
         words[i] = words[words.length - 1 - i];
         words[words.length - 1 - i] = temp;
        }
        for (String word: words) {
            reversed += word;
            reversed += " ";
        }
        System.out.println(reversed);
        return reversed;
    }

    public static void sortArray(String s){
        String[] words = s.split("\\s");
        Arrays.sort(words);
        for (String word: words) {
            System.out.println(word);
        }
    }

    public static void shortestWordLength(String s){
        String[] words = s.split("\\s");
        int shortestLength = 10;
        for (String word: words) {
            if(word.length() < shortestLength){
                shortestLength = word.length();
            }
        }
        System.out.println("Длинна самой короткой строки: " + shortestLength);
    }

    public static void wordsCount(String s){
        String[] words = s.split("\\s");
        System.out.println("Слов в массиве: " + words.length);
    }

    public static void addSpace(String s){
        String addedSpaces = "";
        char[] enteredString = s.toCharArray();
        for (char symbol: enteredString) {
            if(symbol == ' '){
                addedSpaces += " ";
            }
            addedSpaces += symbol;
        }
        System.out.println(addedSpaces);
    }

    public static void isItPolidrom(String s){
        String reversed = stringReverse(s);
        if(reversed.equals(s)){
            System.out.println("Да это полидром");
        }
        else{
            System.out.println("Нет это не полидром");
        }
    }

    public static String changeSubStr(String s){
        Scanner scanner = new Scanner(System.in);
        System.out.println("Что заменить: ");
        String replacedStr = scanner.next();
        System.out.println("Чем заменить: ");
        String replacingStr = scanner.next();
        String replaced = s.replace(replacedStr, replacingStr);
        System.out.println(replaced);
        return replaced;
    }

    public static void subStrDistance(String s){
        Scanner scanner = new Scanner(System.in);
        System.out.println("Введите подстроку: ");
        String subStr = scanner.next();
        int space = s.indexOf(subStr, s.lastIndexOf(subStr)) - subStr.length();
        System.out.println("Расстояние между подстроками: "  + space);
    }
}
