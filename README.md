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
# questao 2
```java
package desafio8;

import java.util.Scanner;

/**
 * 2. Crie um método com nome de converteMaiusculaEConta(), este método recebe
 * por parâmetro uma variável String e torna ela em maiúscula em seguida mostra
 * na mesma saída a quantidade de caracteres que esta variável possui.
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        String palavra;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite uma palavra:");
        palavra = ler.nextLine();
        converteMaiusculaEConta(palavra);
    }

    public static void converteMaiusculaEConta(String p) {
        System.out.println(p.toUpperCase());
        System.out.println(p.length());

    }
}
```
# questao 3
```java
package desafio8;

import java.util.Scanner;

/**
 * 3. Crie um método chamado somarLista(). Este método recebe como parâmetro um
 * número inteiro que representa a quantidade de vezes que o loop deve ser
 * executado. O método então soma todos os valores até esse número e mostra o
 * resultado da soma.
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        int n;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite um número:");
        n = ler.nextInt();
        somaLista(n);
    }

    public static void somaLista(int x) {
        int i = 0;
        int soma = 0;
        while (i < x) {
            i++;
            soma += i;

        }
        System.out.println("A soma da lista de número é:" + soma);

    }
}
```
