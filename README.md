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
# questao 4
```java
package desafio8;

import java.text.DecimalFormat;
import java.util.Scanner;

/**
 * 4. Crie um método com o nome de calcularMedia(), que recebe por parâmetro
 * três números fracionários e retorna a média deles (double).
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        double n1, n2, n3;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite a primeira nota:");
        n1 = ler.nextDouble();
        System.out.println("Digite a segunda nota:");
        n2 = ler.nextDouble();
        System.out.println("Digite a terceira nota:");
        n3 = ler.nextDouble();
        System.out.println("Sua media é"+calcularMedia(n1, n2, n3));
    }

    public static double calcularMedia(double x, double y, double z) {
        double media;
        DecimalFormat df = new DecimalFormat("0.00");
        media = (x + y + z) / 3;
        return media;
    }
}
```
# questao 5
```java
package desafio8;

import java.util.Scanner;

/**
 * 5. Crie um método com o nome de inverterTexto() que recebe por parâmetro uma
 * String e retorna a String invertida (String).
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        String palavra;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite uma palavra:");
        palavra = ler.nextLine();
        System.out.println("Original:" + palavra);
        System.out.println("Inverso:" + inverterTexto(palavra));

    }

    public static String inverterTexto(String p) {
        String inverte = " ";
        for (int i = p.length() - 1; i >= 0; i--) {
            inverte += p.charAt(i);
        }
        return inverte;
    }
}
```
# questao 6
```java
package desafio8;

import java.util.Scanner;

/**
 * 6. Crie um método com nome de conversorKM(), que recebe por parâmetro um
 * valor em metros (double) e retorna o valor convertido em quilômetros
 * (double). A conversão é feita dividindo o valor em metros por 1000.
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        double n;
        Scanner ler = new Scanner(System.in);
        System.out.println("Digite um numero:");
        n = ler.nextDouble();
        System.out.println("De metros para Km é:" + conversorKM(n) + "Km");

    }

    public static double conversorKM(double x) {
        double calculo = x / 1000;
        return calculo;
    }
}

```
# questao 7
```java
package desafio8;

import java.text.DecimalFormat;
import java.util.Scanner;

/**
 * 7. Crie um método com o nome de calcularVolume(), este método recebe por
 * parâmetro o valor do raio. Para calcular o volume de uma esfera utilize a
 * seguinte Fórmula: (4/3) * PI * raio³. (retorne double)
 *
 * @author Henrique Michel Rodrigues
 */
public class Desafio8 {

    public static void main(String[] args) {

        double r;
        Scanner ler = new Scanner(System.in);
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Digite um numero:");
        r = ler.nextDouble();
        System.out.println("O volume da esfera é:" + df.format(calcularVolume(r)) + "cm³");

    }

    public static double calcularVolume(double x) {
        double calculo = (4.0 / 3.0) * Math.PI * (Math.pow(x, 3));
        return calculo;
    }
}
```
