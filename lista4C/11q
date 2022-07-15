#include <stdio.h>
#include <stdlib.h>
#include <time.h>

void algoritmo_rol (int *, int *, int *, int , int);
int diagonais (int *, int);

int main () {
	int *vetor_X, *vetor_Y, *matriz_M;
	int vTam, intervalo;

	puts("Qual tamanho dos vetores X e Y?");
	scanf("%d", &vTam);
	
	vetor_X = malloc(vTam * sizeof (int));
	if (!vetor_X) {
		puts("Falha na solitação de memória!");
		exit(1);
	}
	
	vetor_Y = malloc(vTam * sizeof (int));
	if (!vetor_Y) {
		puts("Falha na solitação de memória!");
		exit(1);
	}

	puts("Qual o limite N do intervalo? (0 até N-1)");
	scanf("%d", &intervalo);
	
	srand (time (NULL));
	for (int k = 0; k < vTam; k++) {
		*(vetor_X + k) = rand () % intervalo;
		*(vetor_Y + k) = rand () % intervalo;
	}

	matriz_M = calloc((intervalo * intervalo), sizeof(int));
	if (!matriz_M) {
		puts("Falha na solitação de memória!");
		exit(1);
	}

	algoritmo_rol (vetor_X, vetor_Y, matriz_M, vTam, intervalo);

	puts("Resultados:");
		
	printf("X = {");
	for (int k = 0; k < vTam; k++)
		if (k != vTam - 1) printf("%d, ", *(vetor_X + k));
		else printf("%d", *(vetor_X + k));
	printf("}\n");

	printf("Y = {");
	for (int k = 0; k < vTam; k++)
		if (k != vTam-1) printf("%d, ", *(vetor_Y + k));
		else  printf("%d", *(vetor_Y + k));
	printf("}\n");

	printf("Matriz M :\n");
	for (int k = 0; k < (intervalo * intervalo); k++) {
		if ((k != 0) && ((k % intervalo) == 0)) printf("\n");
		printf("%d\t", *(matriz_M + k));
	}
	printf("\n");

	diagonais (matriz_M, intervalo);
	
	free(vetor_X);
	free(vetor_Y);
	free(matriz_M);
	
	return 0;
}

void algoritmo_rol (int *Ax, int *By, int *Cm, int nT, int nM) {
	// Obs: Ax = coluna e By = linha
	for(int k =0; k < nT; k++) (*(Cm + (nM * *(Ax + k)) + *(By + k)))++;
}


int diagonais (int *M, int n) {
	int diagP = 0, diagS = 0;
	for (int k  = 0; k < n*n; k += (n+1))
		diagP += *(M + k);
	for (int k = (n-1); k < n*n ; k += (n-1))
		diagS += *(M + k);
	printf("Soma -- Principal: %d, Secundária: %d\n", diagP, diagS);
	return 0;
}
