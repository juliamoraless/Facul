/* 25. Calcule o valor de π a partir da serie infinita.
Imprima uma tabela que mostre o valor de π aproximado por um termo dessa serie, e depois por dois
termos, tres termos, e assim por diante. */

#include <stdio.h>

int main()
{
    double pi = 4, operador = -1, lim, i;
    
    puts("Defina um limite para a aproximacao: ");
    scanf("%lf", &lim);
    
    for(i = 0; i <= lim; i++){
        pi += operador * (4/(3+2*i));
        printf("%.0lf°) π: %lf\n",i ,pi);
        operador *= -1;
    }
    
    return 0;
}
