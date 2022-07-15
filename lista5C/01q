#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[]){
    char op;
	int *r = NULL, resultado, *a = NULL, num_a, *b = NULL, num_b;

    num_a = atoi(argv[1]);
    num_b = atoi(argv[2]);
	op = *argv[3];

	a = &num_a;
	b = &num_b;
	r = &resultado;
	
	switch(op){
		case 's':
			*r = *a + *b;
			printf("Resultado = %d\n", *r);
			break;
		case 'm':
			*r = *a * *b;
			printf("Resultado = %d\n", *r);
			break;
		default:
			printf("Uso incorreto\n");
			break;
	}
    
    return 0;
}
