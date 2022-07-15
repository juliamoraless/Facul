/* 2. Modifique o programa anterior adicionando um campo z com a media aritmetrica de (x, y).
A media deve ser calculada por uma funcao e a estrutura passada por referencia. 
O tipo de retorno dessa funcao deve ser void. */

#include <stdio.h>

void mediaZ(int *x, int *y, float *z){
    *z = (*x + *y) / 2;
}

typedef struct{
    int x;
    int y;
    float z;
}Node;


int main(){

    Node node;
    Node *pNode = &node;
    
    puts("Informe o valor de X:");
    scanf("%d",&pNode->x);
    
    puts("Informe o valor de Y:");
    scanf("%d",&pNode->y);
    
    mediaZ(&pNode->x,&pNode->y, &pNode->z);
    
    printf("O valor de z (media entre x e y) eh: %.2f", pNode->z);

    return 0;
}
