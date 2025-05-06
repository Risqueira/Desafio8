# Desafio8
# questao 1
```java
package desafio8;

import java.util.Scanner;

/**
 * 1. Crie um método com nome de mostrarMaior(), este método recebe por
 * parâmetro três números inteiros e imprime o maior deles.
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        int n1, n2, n3;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite primeiro numero:");
        n1 = ler.nextInt();
        System.out.println("Digite segundo numero:");
        n2 = ler.nextInt();
        System.out.println("Digite terceiro numero");
        n3 = ler.nextInt();
        mostrarMaior(n1, n2, n3);
    }

    public static void mostrarMaior(int x, int y, int z) {
        int maior;
        if (x > y && x > z) {
            System.out.println("Primeiro numero e o maior de todos:" + x);
        } else if (y > x && y > z) {
            System.out.println("Segundo numero e o maior de todos:" + y);
        } else if (z > x && z > y) {
            System.out.println("Terceiro numero e o maior de todos:" + z);
        } else {
            System.out.println("Todos são iguais");
        }
    }

}
```
