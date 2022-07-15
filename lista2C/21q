/* 21. Um palindromo eh um numero, ou frase textual, que pode ser lido da mesma forma da esquerda para a direita e vice-versa.
Por exemplo, cada um dos seguintes inteiros de cinco digitos  eh um palindromo: 12321, 55555, 45554 e 11611.
Escreva um programa que leia um inteiro de cinco digitos e determine se ele  eh ou nao um palindromo.
[Dica: use os operadores de divisao e modulo para separar o numero em seus digitos individuais.] */

#include <stdio.h>

int main()
{
    int num, vetorNumeros[5], i, checagem = 0;
    
    puts("Digite um número de 5 digitos: ");
    scanf("%d",&num);
    vetorNumeros[0] = num / 10000;
    vetorNumeros[1] = (num % 10000) / 1000;
    vetorNumeros[2] = (num % 1000) / 100;
    vetorNumeros[3] = (num % 100) / 10;
    vetorNumeros[4] = num % 10;
    
    for(i = 0; i < 5; i++){
        if(vetorNumeros[i] == vetorNumeros[4-i]){
            checagem++;
        }
    }
    
    checagem == 5 ? printf("\n%d eh palindromo.",num) : printf("\n%d nao eh palindromo.",num);
    
    return 0;
}
