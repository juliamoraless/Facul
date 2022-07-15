/* 22. Escreva um programa que leia um numero inteiro e determine e imprima quantos digitos no inteiro sao algarismos 7. */

#include <stdio.h>

int main()
{
    int num = 0, numOriginal, i, x, y, qtdDigitos = 6, numeros7 = 0;
    unsigned long int vetorNumeros[999999]; //Valor maximo.
    
    puts("Digite um número inteiro digitos: ");
    scanf("%d",&num);
    numOriginal = num;
    
    for(i = 0; i < qtdDigitos; i++){
        vetorNumeros[i] = num % 10; //separa cada digito do numero passado.
        num = num / 10;
        if(num<0){
            break;
        }
    }
    
    for(i = 0; i < qtdDigitos; i++){
        if(vetorNumeros[i] == 7){
            ++numeros7;
        }
    }
    
    printf("Existem %d algarismos 7 no numeros %d", numeros7, numOriginal);
    
    return 0;
}
