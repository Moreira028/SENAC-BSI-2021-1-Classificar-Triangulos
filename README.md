# Algoritmo de Classificação de Triângulos

package Alg.Aula_Algoritmo;

import java.util.Scanner;

public class Ex2 {
        public static void main(String[] args) {
            Scanner leitor = new Scanner(System.in);    
            
            int opcao = 1;
            
            System.out.printf("Digite o valor de A: ");
            int lado1 = leitor.nextInt();
            System.out.printf("Digite o valor de B: ");
            int lado2 = leitor.nextInt();
            System.out.printf("Digite o valor de C: ");
            int lado3 = leitor.nextInt();
            
            if ((lado1 < lado2 + lado3) && (lado2 < lado1 + lado3) && (lado3 < lado1 + lado2)) {
                if (lado1 == lado2 && lado1 == lado3) {
                    System.out.println("Triangulo Equilátero");
                } else if ((lado1 == lado2) || (lado1 == lado3)) {
                    System.out.println("Triangulo Isósceles");
                } else
                    System.out.println("Triângulo Escaleno");
        } else {
            System.out.println("Não é um triangulo!");    
            }
            
        }
}

Ferreira, Gabriel. moreira028@gmail.com.

Data: 05/05/2021
