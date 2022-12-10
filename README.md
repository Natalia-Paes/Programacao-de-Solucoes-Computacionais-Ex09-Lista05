# Programacao-de-Solucoes-Computacionais-Ex09-Lista05
Reverso do número. Faça uma função que retorne o reverso de um número inteiro informado. Por exemplo: 127 -> 721.
import java.util.Scanner;

public class Ex09 {
    public static void main(String[] args) throws Exception {
        Scanner sc = new Scanner(System.in);
        System.out.println("Informe um número inteiro: ");
        int number = sc.nextInt();
        sc.close();
        String reverseNumber = reverseNumber(number);
        System.out.println("O número " + number + " invertido passaria a ser o " + reverseNumber + ".");
    }

    public static String reverseNumber(int x) {
        String str = Integer.toString(x);
        String reverseNumber = "";
        for (int i = str.length() - 1; i >= 0; i--) {
            reverseNumber += str.charAt(i);
        }
        return reverseNumber;
    }
}
