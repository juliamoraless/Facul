/* 24. Um triangulo retangulo pode ter lados que sao valores inteiros.
O conjunto de tres valores inteiros para os lados de um triangulo retangulo eh chamado de tripla de Pitagoras.
Esses tres lados precisam satisfazer o relacionamento de que a soma do quadrado de dois catetos eh igual ao quadrado da hipotenusa.
Ache todas as triplas de Pitagoras nao superiores a 500 para cateto1, cateto2 e hipotenusa.
Este eh um exemplo de computacao por forca bruta. */

#include <stdio.h>

int main(){

    int i, j, k, cateto1, cateto2, hipotenusa;

    for(i = 1; i <= 500; i++){
        cateto1 = i;
        for(j = 1; j <= 500; j++){
            cateto2 = j;
            for(k = 1; k <= 500; k++){
                hipotenusa = k;
                if(cateto1 * cateto1 + cateto2 * cateto2 == (hipotenusa * hipotenusa)){
                    printf("c: %d | c: %d | hip: %d\n", cateto1, cateto2, hipotenusa);
                }
            }
        }
    }

    return 0;
}
