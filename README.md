# Algoritmo de Classificação de Triângulos

package Alg.Prova01;

import java.util.Scanner;

public class Ex6 {
        public static void main(String[] args) {
            Scanner leitor = new Scanner(System.in);
           
            double maior, arrays;

            System.out.printf("Digite o valor de A: ");
            double a = leitor.nextDouble();
            System.out.printf("Digite o valor de B: ");
            double b = leitor.nextDouble();
            System.out.printf("Digite o valor de C: ");
            double c = leitor.nextDouble();

            double lados[] = {a,b,c};

            for(int i=0;i<lados.length;i++) {
                lados[i]=-lados[i];            
            }

            for(int i=0; i<3; i++){
                lados[i] =-lados[i];
            }        
            if(lados[0]>= lados[1]+lados[2]){
                System.out.println("NAO FORMA TRIANGULO");

            }else if((lados[0]*lados[0]) == (lados[1]*lados[1])+(lados[2]*lados[2])){
                System.out.println("TRIANGULO RETANGULO");

            }else if((lados[0]*lados[0])>(lados[1]*lados[1])+(lados[2]*lados[2])){
                System.out.println("TRIANGULO OBTUSANGULO");

            }else if((lados[0]*lados[0])<(lados[1]*lados[1])+(lados[2]*lados[2])){
                System.out.println("TRIANGULO ACUTANGULO"); 

}

            if(lados[0] >= lados[1]+lados[2]){

            }else if( lados[0] == lados[1] && lados[0] == lados[2]){
                System.out.println("TRIANGULO EQUILATERO");

            }else if(lados[0] == lados[1] || lados[1] == lados[2] || lados[2] == lados[0]){
                System.out.println("TRIANGULO ISOSCELES");
            }else{
                System.out.println("");
            }          
        }
            
}

Ferreira, Gabriel. moreira028@gmail.com.

Data: 05/05/2021
